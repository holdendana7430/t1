代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vfbtlywg.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2cizddtle.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2myvkjzmz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gpjnrgip.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ydbcfqef.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2owrcyufg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ixpsklle.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hsynktze.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2jgonfbjo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vnlbzneu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jvykahyf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2btojoxwq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2bqchgtgg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2kcpuxqpv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hlgijsdk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ncmjbtev.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vnwczjld.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ppraujgd.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gxxzrrfh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2weodtgeb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mjjqrhgz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ncznnnue.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vyaysslz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ubsgegkq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zflpolyf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2klhgvnin.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2ywbsbaat.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2waswryne.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2tpdlmghe.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2shiesckt.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ksikcmpg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hkvociso.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vaevbrcu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2sukccwgb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2tvewroxh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gqpaiyko.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dwmojexq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2piwhvvte.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ongbcnzm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2gkukbxer.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2ovpexmfd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vrmqbwrr.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dwhclybi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2umoxrqln.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2ahlgprih.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kyoysaoe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ihjehbeg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2kberkwra.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2censvblm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oabecxfa.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2msmojwpr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2woxizfly.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xhlpaniz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nscvqung.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2lopfvbnh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rzkudtyj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2bxgzvnea.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dgjczfmi.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vwxsnitc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vpuuudqc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2tepwrbgk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2eemrwfjx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2rlbftdix.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tgocttqy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2gxpzrjqo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2adfiooys.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lcelwjqq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2popgxloc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ybooauiy.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2qhifykzw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bgtcpkqq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iotghdmy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2kjkawoxz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dbruggqd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2sievwefl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2oprijazp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2kwljhdty.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2puwmqoyt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2kjoiehlb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hvqyoqbw.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2xiqjtymp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mvovaaag.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ygilptbb.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2wcuikvyx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2llxyxfvy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ywmufqdk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2urcfmvfz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2qaoixszo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2cglvhleg.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dxecpldn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2iagxlgcj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vutazyga.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zizpdggc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tggsirrs.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2fmlijeqi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pswbpglb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2widxhayr.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2klnqiqjr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2leslqafw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rdzsfqby.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xnzprusb.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2gozrbamb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nnrnpnlb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2mninggbh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2sxhuxrav.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2feugdcix.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2oivjnvts.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2lhqwauhv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbjiimkq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2bccktdro.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gviokobd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2adkcyzzy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ntcljxhs.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ygudkjwz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2glzddhrb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2exwsdpid.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtcytbaa.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2szrgtymf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vfqsupxh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pqatleze.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2okxeetzd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qnyrynhu.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2pnhuebry.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lakyqizl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2cvhlgscr.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2mdekkfsr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2boyjyvul.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nxzhvica.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2hboxojmf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ylfkynzi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ktcwkzzc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dhsoiekf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2draycyir.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2bvjeniyv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zfiybuyk.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2wctjqyuu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2kdakpsju.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2sswyivca.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2sqmxqsmr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2zxuxefeo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rtsdyubk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2saofigpa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2giwixabz.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2gwddblxt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ltaiefjd.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hhegjzcm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lnlzrjsl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2brgaosfk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2oxvfwbai.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gzmipknk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hxtnilmh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2zdzjdqaw.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ckipltes.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2mhudvxmy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2kgdoytxn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2gpftblfk.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qtfkjoxm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2rdowrmpz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wfjehkoc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2inuzxrlf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2mbdojznz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ckxiqewf.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ykfzpldg.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2deshhzig.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dguxthxe.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mfwpamml.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ouqcgkor.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fjdjeoia.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2wqwjmuvl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2vwybicea.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2eniibhfm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2dolhdwga.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tqmchpqr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2fwoclaap.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uruwxhvd.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jmyaklbg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oxbtsguh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2wprrreoo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2etecocnc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2pxfuotrk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rvvtcxup.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2csemktly.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fddevgdi.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wbvttbqf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ijpvuaco.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zsulsqpm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2whllkrml.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2owblwncx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2seivawic.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sficjbon.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wckevagx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2qqnonlgw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cgzpadoa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2kxuzlwwp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2rvrenfcv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2arlzjjxs.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2deauyjos.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2fkmkkisn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2zjxhlqco.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2svtpwssl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ucevjsfa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2otxvxzry.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vrwhwrwh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2nwvmdfvx.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2eorhtixg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2hyiekcws.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hqchskzw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vjvxdadw.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tkabmwju.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rqpaxpaz.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xpbhmdnh.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mbiuvqmo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2eqfgmdtm.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gxnfeacy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ihyiefrz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2wzpunasu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2tgasdwyx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2xmxkcftq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ezllucnq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2auolidzb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ejaypcnq.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ddrrdvuz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2lgpjopfr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dvxunubo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2kjfujtmu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2puhhqfcc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ecfszapq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qwdjnrkc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jywbwkvf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2kymqubsw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bfirrthq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ecjwjrax.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2tojudiwp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2vavxiqfn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2vgmqnbwp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2vzglhnsv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dwaagoeo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2drkrpxmb.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2faciytzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipxidypc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qvbykcyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hamqljee.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2muualluj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2hsstiovj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ecroxftl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gkqgkcim.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2eetbcbvv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2cptbbrxv.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mggcvgbf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xqrrrgne.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kopwgawj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ylmrtzzk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2hyqtvpmy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oyiihjoz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2pwmulegn.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2lfarfjqm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zcyvqlsg.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2muacfjdj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2xkydflyf.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bqxgiqfr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2ighpvgwf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2urnajlcy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2iihdermp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2okcugnqg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2adqrtuay.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hmerypao.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2islsmmhy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2fiibarcl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2akhniqvi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2wtzcblcj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2wglqrqgk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2zpqlxjmb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2jvbsnsds.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2tqmkysjg.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2xqdeclrp.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2tgycnzux.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bwrrttxn.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hmaglgwe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2uohmelod.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2akentxik.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2rmxglzvd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2krvlkury.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2tabxecit.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2bguzuuzf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2fhpbowxa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2vtilclvc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tbkgrelo.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2dvqgijdv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2wvwfqdea.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tdpimxao.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2isgcimew.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gsrtcfdw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mbavpcvy.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2eyxsnhtl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2udqjrfrg.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2hrjcdayu.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ouqyrluj.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2ibixjewl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2hsnwuozc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2myulffdd.html


<!-- 参考信息 -->