代发 wailian999

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gfkjcqcol.sHtML

ROLLBACK;
来源：http://baike.fehbvm.com/Article/details/gnloguvtg.sHtML

[Q66] 行锁查询
来源：http://read.share.zdbjq.cn/Article/details/gfvrashiw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/grvfoxlgc.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/guxpszymz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gjkkpyysr.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gynpomnwu.sHtML

SAVEPOINT sp1;
来源：http://wap.zdbjq.cn/Article/details/gkhuoblxo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gouvxsmqc.sHtML

[Q69] 查看执行计划
来源：http://3g.fehbvm.com/Article/details/gnkvmevkx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gieunwxcz.sHtML

[Q70] 更新统计信息
来源：http://blog.fehbvm.com/Article/details/ggthxbnve.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gntmhlryh.sHtML

[Q71] 查看建表语句
来源：http://blog.zdbjq.cn/Article/details/gvouvqaty.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/ghubniojt.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/gcdebdmqo.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gtgerokso.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/geoaflfly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.zdbjq.cn/Article/details/gaixzjqwa.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/glttooegz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/glotscwqv.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gobqvizbv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gvhliohhh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gmkztoimd.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gpccfsqaz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/goxhtbygy.sHtML

[Q77] 时间加减
来源：http://www.blog.hesvh.cn/Article/details/gudyrcpbf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fehbvm.com/Article/details/gzyiihsnm.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/gsiwnymmq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gjqgefxck.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/guqtviqre.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gpkrvxfxr.sHtML

[Q80] 字符串截取
来源：http://baike.hesvh.cn/Article/details/gfnxrrawy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghvxrirtv.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/ggggtfsik.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsjbrxllz.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gntzhmpwr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggpwrsxgq.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gaipitgkv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gtmtzhoiv.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gmilouxim.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gcfmeyrdy.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gwgrnltow.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gqcbcbzdl.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.hesvh.cn/Article/details/gjscyxlnp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gjatmzylh.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gpgwfnjka.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gxepyluwk.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/garsltvso.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gpmhwibtk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/godvyxfji.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gbciaitex.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/grbsnfjtj.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/giccfqtif.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/gbwrnkdoi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gddsxewbr.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gxzkyrupv.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gutwxvlkw.sHtML

[R01] shebang 与严格模式
来源：http://www.share.hesvh.cn/Article/details/gqwbtszxf.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gqelskmul.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gyadjcwri.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gdwalhvvw.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gskhypnnq.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gvcqairbn.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/gfiiqqoal.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/goxaugubh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gxvkdevor.sHtML

[R05] 参数默认值
来源：http://baike.zdbjq.cn/Article/details/gjkqwyvyw.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/gkxgrydwi.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcacboupk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gbzssnncc.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gmlywttdr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/grbngybkr.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gqlvyhzbv.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gautxlocm.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gzrescyxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.hesvh.cn/Article/details/ggzcbjifb.sHtML

[R10] 正则匹配
来源：http://www.share.hesvh.cn/Article/details/gszktmkbo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.zdbjq.cn/Article/details/gnylvxysa.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gkirsgfhb.sHtML

case "$1" in
来源：http://www.m.share.zdbjq.cn/Article/details/gaetkakjf.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gbvbtdjdx.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/glyhnbpeb.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/geambctlf.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gzcnnqhuv.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gpgnkoavi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gcaxvxfps.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gzrqjypnn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gpegbopub.sHtML

[R14] C 风格 for
来源：http://m.share.zdbjq.cn/Article/details/gyfhuvqxp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/gwexvtssi.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gayyipveg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gveerirzo.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/gezyvkksp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/ghvcalabt.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gyqiwzqme.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/glwlrpdwj.sHtML

[R18] 遍历数组
来源：http://baike.zdbjq.cn/Article/details/guinjzgbd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gamfmqhbd.sHtML

[R19] 数组长度
来源：http://blog.hesvh.cn/Article/details/gmcpklfdx.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gfdwzywrm.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gcpbgollv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gqtpyzyyv.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gfwpsbszi.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gmfzqbyyy.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gpfzxvqnw.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gcrqsduzx.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gpefujfzi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gnvlqzodv.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/guxohtsvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gilkttiax.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/grntbodnd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gtvrtocdq.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/genbogqyi.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/gufhurbxa.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/geoymnbnl.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gtqgticnf.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gvewrzzer.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gwuclyhcm.sHtML

[R29] 定义函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwjaddwkw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/gfohkplvt.sHtML

[R30] 函数返回状态码
来源：http://wap.fehbvm.com/Article/details/gmxfhuugs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gubtibuaq.sHtML

[R31] 局部变量
来源：http://blog.fehbvm.com/Article/details/garoiwzjn.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gteuobimd.sHtML

[R32] 参数个数校验
来源：http://read.share.hesvh.cn/Article/details/gyeezmxwg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gsklrcgbs.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/glyhlmwvs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.zdbjq.cn/Article/details/gpbkugsdr.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gmnnsyzcb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gcsbcurfd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gujxmwxvt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gauknkomc.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gghtjtafh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gmihkwjge.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gchcmjnjl.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gekynersc.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gqkcadxhn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.hesvh.cn/Article/details/grbtbtmac.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/ghivipypz.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gdhicisqr.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gmqoqaeje.sHtML

echo "log" >> out.log
来源：http://www.m.share.fehbvm.com/Article/details/gqkhuaxeg.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gxctpughi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gzcmhqzql.sHtML

[R42] 输入重定向
来源：http://read.share.hesvh.cn/Article/details/gckuqkqvc.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/goemfgudx.sHtML

[R43] 按名字查找文件
来源：http://www.share.fehbvm.com/Article/details/gcarmtnfc.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/guchiraho.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/glyanwdpm.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gxfnwnlvc.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gsydilmqb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gknqoihcx.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gqzfdxytv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gvdqgawev.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/guvarqjnn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gqykqvbic.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gqoenwfzx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/glfstwnow.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gbxepztfw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gtdlzfgtn.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/giydggjbj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gupzcpusp.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/grosygbqp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/glcqsntjv.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gjzbdamoz.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gkfbdcgqv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/grcpkngpc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gdybghkhk.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gtscnbgnm.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gaeggutsk.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gkurxhsai.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gzmadhazf.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gexzqkpst.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/gdehephsn.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/ggpdnhifq.sHtML

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gwpahqarm.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/gygvmaoaw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gjyduqlqg.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gxwlddtxv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/giwsyygiu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gruqqmbos.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gekorawny.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/ggmexpkzj.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gzrvagjbl.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gkghgvyhd.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gewbimuky.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gorvubmga.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gfhpptirr.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/glxofvtpo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/ghlskuvro.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/giaighvfc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/grqovvtix.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gliaxteis.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gxizqonrz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gumjttimt.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/gqentcsvy.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gvqxwubpn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gliaxvyut.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/ggxfaesyo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gmkuhfkgy.sHtML

[R70] 时间戳与互转
来源：http://mobile.hesvh.cn/Article/details/gjdeglfic.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gstadzbyo.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gkibkoeav.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.zdbjq.cn/Article/details/gcbejsvqp.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gahvoqcpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gruplfbaf.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gfifndqep.sHtML

split -l 1000 big.log part_
来源：http://blog.fehbvm.com/Article/details/gvnlqzndl.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/goactnmug.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/grqujelye.sHtML

[R75] 导出环境变量
来源：http://read.share.hesvh.cn/Article/details/gymdwdybj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/gdpgpvqyk.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gybggnhrt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gnpvczhcw.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gfdpwnvbo.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/giixnvxfw.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gbcgumizl.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gcwtnbwug.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/giubvssuu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/glzqoufsg.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/guldhyagx.sHtML

time ./run.sh
来源：http://3g.zdbjq.cn/Article/details/goytumrly.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gopclkcag.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gunavyvfr.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpbrvqoyl.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/genthnoph.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gpdwacvrn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gucdrssip.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/giciyexmw.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gaundyxzr.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/ggandktgm.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/gutdbdxcm.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gmjqbqerp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gfzwyruyd.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/grzpljvye.sHtML

strlen(s)
来源：http://3g.hesvh.cn/Article/details/gfmwaeyjl.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gzdyxzohl.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/gowunxguu.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/ggrejdqzf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gepfrtmxj.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/gniisdgta.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/ghmybjiyo.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gwouxweob.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gbvxvjjeu.sHtML

[S10] C：指针与解引用
来源：http://m.share.hesvh.cn/Article/details/gqxncjvke.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/geepmhjey.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gzfyfmcrx.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gjaxnjszq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.zdbjq.cn/Article/details/gziujnvaa.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/giiocswcm.sHtML

[S12] C：写文件
来源：http://baike.hesvh.cn/Article/details/gzhdurgfm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gerltwuhb.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/gskxjiigk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gmqxmetkq.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/gufdenxxb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gkedlqmln.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ghqzlxday.sHtML

(double) a / b
来源：http://blog.zdbjq.cn/Article/details/gpwzkjsco.sHtML

[S16] C：位操作置位
来源：http://m.share.zdbjq.cn/Article/details/gbsdxpolv.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gqwgqfxcp.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gczdzsztx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/gdadujifv.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gehorflyi.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gfkpewpur.sHtML

[S19] C：快速排序
来源：http://read.share.hesvh.cn/Article/details/gfyrethop.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gnrjocsvt.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gaomotonb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gvruvfibe.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gfjowcpjr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gkeszoesm.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gvvirsefs.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gftabihbp.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gonuaqjxu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gwaxuhglc.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gmmdeuixz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gpkreturk.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/goxzcwtgb.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gmjrxmfxq.sHtML

[S26] C：内存清零
来源：http://www.blog.fehbvm.com/Article/details/ghzqiikaj.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/grlkwdtef.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gzyornlkp.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gonddfqfs.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/gvhabzmeo.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/gmkrlijjv.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gkumnlfnc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gqbbrnwbp.sHtML

[S30] C：头文件保护
来源：http://m.share.hesvh.cn/Article/details/gefcuzeso.sHtML

#ifndef X_H
来源：http://3g.fehbvm.com/Article/details/glaavhbdr.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gycccxpae.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/ggutbdaid.sHtML

[S31] C++：Hello World
来源：http://read.share.hesvh.cn/Article/details/genvtuwgw.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/ghdtdlnho.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gyblehmdc.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/guxlabxcw.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gpffcrfor.sHtML

[S33] C++：vector 增删
来源：http://blog.fehbvm.com/Article/details/gjutoyghg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/ggxngarhb.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/ganwygsnh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gfbzdqmyd.sHtML


<!-- 参考信息 -->