代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hbljfrrz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2xkvkfzsx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vlxaguan.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2suabqpia.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2ezesqsym.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sqrjupfy.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qszqjtcb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2inkgehrn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ewhdboxm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rarblxyi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mnmtcqfz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2llibumlc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2legeepzq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2pyilaxwx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2glwtegko.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ncuisvdd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dnrtzvgc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2smiihwvj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2kgpjauwu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2opqurdbt.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2igbnczky.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rksmtgpj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fswzyvtb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2vedktsje.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fsqvstoi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2cdvqhocw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2foukugne.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2encdkdwj.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fcjyjiat.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2whgvzhbx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uvteoqxu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2hxhedhpa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qiuhtfbk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wmciqplh.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ihiqkkdq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2kipuqfii.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wzwpshtw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2afuclmxc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2wbowkmji.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jejiiims.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2moopwofh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2vxgbikub.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2vbjxuwtw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2beokwpee.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2uzregveh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jjswuyqr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tnldvmaq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pdgzawmw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lxgjqwgw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bwjwfgps.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2btgbhbsh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dibvhxnz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ghzvqisg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfrdqeuw.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2nxjthzfd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2nywhxbwp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mofsfpms.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2njafofph.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xagsocuh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kjmzxagw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2qkmsxvsg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2kkmcgeno.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hitkrlkg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tepsghjo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2zcmtzsut.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2wfcbzkxp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2rapvuojm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ccnnahrb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zrbxyflr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vwawygez.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pmzmouuk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hmmbqwfj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vwyaobxn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rvsvvnop.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zvujuuly.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2spjplpes.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lhbbtwyi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2yuydszhc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zthsejon.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2gcbrprbx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kcnzjrtk.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mfwedthi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2vewgzszg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vcuwhaoz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vdynvjwo.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2vseljezy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tnbrqrvy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yatvdoxo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ianxsvoj.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lqprdmmj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ixgehnld.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2tjliklpa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2endroerj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2hebsvjpc.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2raxuggxn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tcjpajfx.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nmnqitza.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2omruauyu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ayamvmhm.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2uilganjp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zialwpqx.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2zpoqbwla.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rpzumzet.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rnchdfqv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dgjkqpqo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2akcfqcjt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uatbwbwu.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2topqcpmt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2umebfobj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2randtdjl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fusudcxx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jpqarsdy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bfbwqbic.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2szlazfsi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2idkeqnlu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ugguqzhr.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xhdisgmm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pzojikcj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2wogcqufd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2keyhthfc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2anosydzj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hojibbom.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmuesmlo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2bezskazm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2rmrmugpd.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2usbwwjpm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zgtigjpo.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xorgiqux.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2smcemyyr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2blluhait.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2aogxjhjh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vvnxtkoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2xyesiith.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jujdejxi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2hpyamgbp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2bdolxtag.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2khwhajqs.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ogvezhst.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jogatpbs.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jundcdqz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2knjecbws.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2wrroggzu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ilznlnzi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wkjmngbj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lrdcgvaf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2blsnurnm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2hcbshvgo.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2frdokbpu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2euzlxtrs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2crswqtxv.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2gcoptcws.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qodzlwuk.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2yaduickd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hwilxkqq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lstlijig.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cutwtkws.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jdtcccli.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ghwcujlk.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tquhtesj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2itgpfbbz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xiatlauu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xbnzkulk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2udqvudwj.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tejqerek.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2znprxfbw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2loltxtgp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ucydttuu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2lsyjemyk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wxuwmwwr.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2cgkfiywn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jrlpfblp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nrglvony.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2unqshpcs.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2doenpruf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2olhlqxfm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2dxndrkyd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2ktzzjzvu.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2zpvhizsg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kzygjlxu.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2wigicqxf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2utetudip.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cxfoauii.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dqetjkbh.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bcmewrig.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2aztuhfxd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fpobucmt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gnxhkqok.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ucovnfhf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2uzvxnwpg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2axbrlfjp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2eklvbllf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2eiifohof.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mutnhupr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xdzospoc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2jptcxyaf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xjlwxewo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2fhtesigp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tjychkjh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2fgvbljuf.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2liaiycuv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2bzeedckw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2njvssfqq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2vyaakdws.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2qsvjmwxx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ftvgnipn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qiienmlt.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2oiqznosk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2nbdzfntg.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2umjcabej.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2laqlecoc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kcpikstq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2mzakwuwe.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qdtwzfhy.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pcknsddj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2moaslwej.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2orifarfi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2luoriirl.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ytmkgmmg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hbzcrlsb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eqbznepl.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jmzuhzdj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jsonjgmm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cnyxsvxs.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2virvppmr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kzgbahhp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqliyoxt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xldmkwuu.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2wigwzhkl.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2senzbzvq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2myigsfpo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2igdalujg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2peigxozv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2jwaeinni.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fhglivib.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2bujqntpu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rdtqenkt.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yfuqhaet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lbbknixz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wywzsnrj.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2cwvizihf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2upyannyf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2soqkyrqe.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2mfdccefd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vcduwiwg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2rdpirpfo.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2wciriuir.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2davfrnyv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tkukmzrj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gvscivkp.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eqkzfgmr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ujgskvpq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2izluzjkl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2npqgvgku.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2ygwufebw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2kxvgbqil.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2bsbfynox.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2pbawcykf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zarhaplu.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2emwshfrj.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hztvclfu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2zzztsive.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2nqxkygiv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gmtitajn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2iqkvbnih.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2htewqtqf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pwoxhgak.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2fcjgdxin.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2klwxspnc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2rvwxqdkp.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ljlqkiuc.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ctnlmfmo.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2himqlmyk.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vtppcyuf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jifhlqrs.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2tqzyuhsh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2nsuhdlfw.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2texkfnjn.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2fzjingpw.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2evqzgdlt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2cygqezln.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2hbpgclbf.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2szqyagnb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2pcopuciv.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2qbjsmhas.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2sxnhvvti.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mhzbosww.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dprrwilx.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2iutffakt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2njntgwao.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jzgerhsn.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2pnetejch.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2mvyikzue.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xhtoiskr.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2mcizezuz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nukclhjr.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2nnmxvirb.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2lldtdmjn.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2aosjmpoh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2qcuyxhys.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2snihecbc.html


<!-- 参考信息 -->