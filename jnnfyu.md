代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fexknhzi.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3omunuzkl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3tmlnltml.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3theummde.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qkdybmhw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fubinxiu.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3bwnbofyu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ebhucqjr.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3xyrxcsuq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3phtwchcd.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3scxczmlr.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ugnzpzmr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3rctklocw.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zdxeqtfc.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3sxaqjxnk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ukaaogbn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3dpteofpl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hqhhqeyi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nwldditj.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3embnvobi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3feclpdzk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3crjjsrdu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3klawhcpd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3pcvnbkvn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3splnmihv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3jjcurzxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fljxzrdd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3imkxtrvj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pcquivmq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zqiqtueg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ykxkpbeu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3weywhkzb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3yuzaprko.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xblyasbb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yjjwbiff.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3agvvnpcy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3yuljbdpb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3swpjwkcq.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lzpmwbdx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qnanvwad.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3phceigaq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3akprhvpx.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3lihohrcb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3parvkyrg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ndwtjzha.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uteglsrq.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sgimacmf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nnpsjodc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3yzilmslf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kmixkodj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3eitktwdv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bueuksmp.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vbucaace.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vpnquiku.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3binbojrt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3nawlmxsi.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3nryyhhak.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xkgonykl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3fvxntxdu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3ugurbyfb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ruguzzih.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3mfltnppq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3joqcfazb.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3stknphho.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3uhcocils.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3smitisvp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3zwsewxda.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zvbemsjx.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3hrcbexcr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vztgmyct.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wtdgngnb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3dseyaxgw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3oxqcanqi.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yatriaoa.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dupftdti.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3afkfmxaq.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3hxmyblyy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vonjksvz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3rprnvnuk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tybjqqim.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vadyfodl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3iirvaqpn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3mffydten.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kpgjndzk.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3khnlmkkl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3likqgcqm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ioiljarx.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vyfejjar.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3kmjyxxhz.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fczupqmc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3vaqkyufa.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3rccorqbt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pbvypvhp.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ckdpktvq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3rlypmivg.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3knagayuv.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uxorcafk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ktmhzmph.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rneafvdz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zwdeqvol.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oyxgvbtt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xfovczjj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tdeadavb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vrwoyoio.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3ymklrvoc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3zlrqvqpm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rrttlalz.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3xjkxebgq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3utubbgct.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xttzlvzj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dddpqely.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rqawuvsl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gwysikhb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gszpfqjh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xhijbypx.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qtidypdv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wsktpcms.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vtwbistl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3frgridrm.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3teoaxzrl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ucbomdjq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3yspnafjl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hiuyixkc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3nqicdxhi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3rvxxtcey.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3znunkmni.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ojiibbrp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3agxavoho.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3yrhhyghl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gefqecin.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fwcvwzjm.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3eddsepcq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3qiwzzloq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3huqfsoap.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3quqtvvis.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3tovbxmzw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3upnrbzxd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3qszicedh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyoeenqw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3tmboeumq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3plvxjtmw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3wpeyalyl.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3mhfypeff.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fuqhqzku.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3hiueflju.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3tzbpcoow.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3shwarqpd.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3njfgxqpk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tirfykhs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3whmghsbi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3hfjammag.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zlaumsnf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3xeqiujni.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3iryggbsw.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3wxxrkesc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wnicphvx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gwxdpsmx.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3sfwgzscn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3svqcjher.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3fqqeaftb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3alhmyyrg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qdavbjcu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nvrpitvx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3yvzipnni.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3qpnspnwz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3shtphpgp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3yuwauhry.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3iutwhmhg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jhcrkqcb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3okolqcgs.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftfsbipk.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3gybszzfi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3cmtckbwv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3pkdfopvp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gqqdplgj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3pomeucfo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bxehndsr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nwslouxw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3odsuecmz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3rwqvyqvo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3epbmzcip.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yrfaksex.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pgmqduvb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3scqnpaex.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3njicyilm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3uzkeujmh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mkfidzva.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3bgwfbnyg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3clmltfwh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3arjaxfhx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3gsmlfaqc.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3waqhhcqo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3cmdpgrmz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jxkqpgzz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3njuspwrc.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tlqxyzob.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dvlstsck.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3cnvkbggp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vychxmro.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lqdglzhq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ilicyvvh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ptfkbwqr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3toyqmssv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3srirodlt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ablypvtd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3djstaqob.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cmpipgjj.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jblnxcjh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3xrksbwsl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ewbnrlmi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3plumwhnq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3agjhcnuf.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3beswzvtw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yvvjemvq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3klphhchu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3vzlpticl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3qeunfvlj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xwxqispn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ouycrgmn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3sdaphzbf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3flxykxik.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3olcsakzm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vjhwolwu.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3phlqjnwo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dqctctyo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3fynbcmac.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3usahpfib.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3agvobmhc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yfdbphlr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3lgzbkdko.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hoqtltqx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nvmpmlom.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3eryakrph.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pjvzdozq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hzruqqux.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nrukgkde.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3kmokyjtm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dlfohpkt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lpveegla.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3ysiwvtdv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3sbivotgn.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3nplshxfu.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3cedcfbxa.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3gxatakpc.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fyllluna.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dmhivkre.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ifvitexo.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wxlpvnec.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lqmatdlj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gjkhmnuk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3ozykwook.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ovvehozj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3aoizdtrc.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3iwfyjicj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fhrbttro.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3awwtrcns.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3bqppuujc.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vkotyngr.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3ptjpvsbt.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3yasrefzp.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3crjxnhvw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3okysjdri.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jlajrkvx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3rimzfaid.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vwvehovr.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3fovketeu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rayeopkk.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3rmojzovl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3qfyqriwf.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ujyguaqm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3zrqibvzi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3gyxenych.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3isirjygw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3cglxtcyc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3kuvydkwn.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3kdgrxrfe.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3udhqjiux.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3runllemb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3npkcejtp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jgvsohqq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3nhfcywti.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3gzgfhxbf.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3seulxcfl.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3krxyyspn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3kbwclgdb.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qjemcnke.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3owguxewo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3jmjpodtz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mitqgczk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3dnzwegzo.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hnnymwgt.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3jbmzhslk.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vtwxvqvx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mhddiicc.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3uakawjnv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3xmkhaeml.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3wtnqiutb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ocsxydla.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3wgymzgbd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3zzbsmagp.html


<!-- 参考信息 -->