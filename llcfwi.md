代发 wailian999

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sapftrsw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yygjwoqh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2igicywze.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2tcdhvrnk.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2csfytedq.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ziiqpxqn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dypchehh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2aonkrlot.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2wwxgreju.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2dpxwqrve.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wpzyudmp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2xaqxcyvj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zsaqlwfv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2omaisurb.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2secbkjmt.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2oguylnwx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bnhtwutz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2npcnufdf.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vtzpkhvw.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2eicxayzq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qrplatti.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2aqnrvmzc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tpoeavbn.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2zpbmkkrp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ktitawlq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pxpvcjjj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2immphctz.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2wcnsrepr.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bveflwmy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2lkbrcooc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sivmebqc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ksnstszi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2zpfcpzoi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bttwknls.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zzwkxbwo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2iuiabpru.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2lqwvbord.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2npwfqfey.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mbbxveau.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2mxgrxttu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2lsprdznq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2injaococ.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2emdyrjip.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2odbsbvue.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2mivknurz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2whualmbb.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fpkswcnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fspptxth.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2bxenoqme.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2upzoyelw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qladmqlo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jipwhihs.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2sugezvyc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kebdysbs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2qhtolgfp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tmfiybvo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zazoyehf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2bwbicfuo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ettruvac.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2wzvqdvsw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pwkgclre.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2uptdwohv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vwovhhgw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2azcslczr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kwkjhsxb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hxwsxuvj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2tarofvsw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aylvxmou.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2vtcdnpcj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rzvxxvap.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2cgfafwyc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2mzsktzdt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2avzmzbgm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ymakswyf.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2hhfscfex.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2zhklgdoq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2rrrudewy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2kaxtcnmp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lxphtubu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hdssxffq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2eopunpdy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ovkrmhot.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2urpakdrh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkyjjxdf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2jsjxkahl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hphzykyw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yhsgijaq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2blnomiob.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2advrmkvk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fyocanwk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tzcvojxv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2bzmlbpdq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2lunofzkx.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jlorasyk.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wfcbaeci.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wevqeqhn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2upsgmgpf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bhgaltly.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2qukseaub.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tdeurzyp.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2hyvbwpxy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wciliozl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nkgsdbsy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yemtpmyv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2folmbwoa.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2imyhgrpl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2krufezld.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lsxogqjy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tfdfylys.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2glbkgvfd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fnvpthtz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2xyvnhmqj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2gfqracsc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qvoirpmv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2wuhjoqqi.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nohiiuww.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2wcwztlvz.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vyqlxdxm.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nhynvegg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eycnuikn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gbifalsr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2chhlqjvi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2eceoxcur.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xriixrhs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2expzimii.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2rxejmohw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2egztlrbv.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xdnebmhz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2bnfnslew.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2lttbeaqf.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2iamaeroh.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2tfnabhtq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rpsnzddb.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ehewwcjn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2qtcpsmtn.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wophzrxe.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2jjrsyvbr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2iwlegefx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gjjcfpoz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xqzpzotp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2cfizkfka.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rpvkcqzb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uqifgrwf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dynrmziz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2sybigvox.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2wyeuxjfy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fpbbfnsp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mvhlcyyj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ytucdzlk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2teyapvjs.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ojkezegv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2bsuevcpw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wlevjnap.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2hfuxkasu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rrnegpna.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2moxbydxg.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2cbpjmypp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2yvapyova.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2odalxorl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2lujcfqsy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2mjfwpyvi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2agtqkzib.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zpwzedss.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2uyvjqels.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rjalrubo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qfhaiici.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2nrfnkiuk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2iecmlumk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2piiuhmth.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ebdgbwxg.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rczmgdya.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2pnfcnkvm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qnnlnqpy.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2asbraake.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2spaobnoc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2fjozrbyi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vwseazrb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vzgmhmdq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2obkgxhkl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ezndaata.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zcnbznxp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2crzzjtro.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rhzqsofe.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ywzipuyc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2qtaxxqea.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2snkwnwlu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2jmobggbx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cdbagazk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2rryhvaou.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2fufiyzqd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hhxjpvto.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2dtzdbarv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2mnyvpslo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2krligmqw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tvcalqbx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2idhkoonx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2qlvkbvyc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2npuxlvit.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2shvfzwku.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2wciegzib.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vpfxrvvf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vlupgmho.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zhovbrph.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2tfgmemoe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qfwlukri.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dkqmhdqd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2oyyupjyf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2kcvgbwyr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2urdcaaox.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ijpflbne.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ukmliozs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2gazobqiq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2cqiaxwzl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dzmavpcb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2hqweugse.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2attqtiim.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sitsvbkx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2ndzzcihj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lcaqeesu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2eohzddbs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2jrlfslfr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2psjedfem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2cjztzqxi.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2fvyedknv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vboatkhf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2plqftgbv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xvfbyuqn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wsydqigr.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2vkjklbxa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2evzdksja.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2tplextjn.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2jtqsrpdf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2esghzcxl.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2hhvebmga.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2wdoouaxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mryjgish.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ulpinayz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ayzufbub.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wzbmveso.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2dqfbypgt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2xofyvjls.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2gnxpnlcr.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2qdaxdgbm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fquluern.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2ippypaik.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2zrebotqn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2njalnqcq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nbzkcatq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vevtjgtz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2pdxveykn.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vmzsdrbh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2axfnpbnn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ywuiadac.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vtyufuwb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2sujqpdxi.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2ggdzlmmk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2hlbivlal.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2owjbfiab.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2cjyfdtwi.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bqvisklo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2syinchfh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2zselodpl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gnxcmiiz.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xsizrhbn.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mmagdsku.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kwomxmgr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2ueepdxau.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ytuasrih.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2tmghxkmw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2puogaleb.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2cxmcwoql.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2atnuvoxg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2jzgjipfx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qriioohr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2ptgtjadt.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2dgllwqss.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2alnlgjkl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2nfytatvh.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ltpxhmol.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2xbdxuwjd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2duipelom.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2mharxwnt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2holtusmu.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2mkudxztk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2cqnrvgpc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2kyvfuzzf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2bonncobg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2vvvoeyuv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2qxwjjadk.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qyzpdtpt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2tcxfsgsz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jmnyogtj.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2oxfeslqu.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2bsnuhdyh.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2bfrbalzi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fcauxkak.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2yvmwjztt.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2apajxths.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zszrrsud.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2fkpmbnkn.html


<!-- 参考信息 -->