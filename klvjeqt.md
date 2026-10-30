代发 wailian999

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/ggginwbru.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.zdbjq.cn/Article/details/gzqkcejns.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gnfdvoazs.sHtML

[Q70] 更新统计信息
来源：http://m.share.hesvh.cn/Article/details/ghnxosvin.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/grjxgqvsa.sHtML

[Q71] 查看建表语句
来源：http://www.share.fehbvm.com/Article/details/gijqyujjj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gxownaorc.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/goucfmznp.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gkycfyaxk.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/glfozpmiy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/grheezuws.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/ggcgqyocw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.hesvh.cn/Article/details/giwukusdv.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gvimkvasc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gabbgoays.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/gqmclbplt.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gxxjcbiid.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/guosbuuec.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gnoekvygy.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.zdbjq.cn/Article/details/gkbskxjwb.sHtML

[Q78] 当前时间
来源：http://www.m.share.fehbvm.com/Article/details/glkwfyjge.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gciyoljpw.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gbicspgmg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gwtkthavl.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gmrrjediy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ghovbnmik.sHtML

[Q81] 字符串替换
来源：http://www.m.share.hesvh.cn/Article/details/gwnyqdhsz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwzawtlmb.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gftobxljh.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gghkbvvip.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghxeatmue.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glymnovat.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gtjehmola.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gnealjlva.sHtML

[Q85] 数值取整
来源：http://baike.fehbvm.com/Article/details/guxbvapwp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/grjuhawut.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gmizamwnd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/ggswjppmx.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gwmrlyyle.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.hesvh.cn/Article/details/gihvltlqz.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gjzxbgftm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gmlmsdfds.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gwvivhbyq.sHtML

[Q89] 判断表是否存在
来源：http://read.share.hesvh.cn/Article/details/gezlxvlhl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fehbvm.com/Article/details/gswcblmjq.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gpqgoiphz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gwbvoxdbo.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gcguirdci.sHtML

R. Bash 专题
来源：http://m.share.fehbvm.com/Article/details/gueqqzkom.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gwghjfquf.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.zdbjq.cn/Article/details/gpvbnausg.sHtML

#!/usr/bin/env bash
来源：http://www.share.fehbvm.com/Article/details/gchtyombz.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gxouslqyd.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/geixvdxzn.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/gpgglovyk.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gybswidgw.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gdsgmkwij.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/gdryviest.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gpjfcakuv.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/giczcrmzb.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/guzxxuvns.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gimvqqlff.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gojhiuzea.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gbgdagshp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gznnmthyy.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/glgyrkgcm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/glvnziptt.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gaxvoqccc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ggoaakotk.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gummfjroh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gwvrdrqmp.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gyrfpzgrv.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gvrtwdxne.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gjcpojttw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gxfmcqrii.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gxvchmfxi.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/guvywokbj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gffnkuiwq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gnupnblix.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gmwvbuuqe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/guodlcpxb.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gdojfpmcu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gycfpkiek.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzvawwtrm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/guijuxznu.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gsweahrzw.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gwkenhurr.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/gcwgwtkhw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gglbygfhi.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gssscnsnu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/ghzpaqrvk.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/gptjepxyi.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gddndcual.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gybeictlj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/gdqcyiqqo.sHtML

[R21] 字符串长度
来源：http://baike.zdbjq.cn/Article/details/gfyshxwxu.sHtML

echo "${#s}"
来源：http://3g.fehbvm.com/Article/details/gjpsitxzd.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gioginhnr.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gqwdrzsjx.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gcucrvpre.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gyuykdjve.sHtML

[R24] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gimhodtvx.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/geydisdxj.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gqjzksewj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gyrjqruyw.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gqfbahbzx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.zdbjq.cn/Article/details/ghmwmpufm.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gbefegjxx.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.hesvh.cn/Article/details/gsmjhwgtj.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gaohjwcfn.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gdotlcuaq.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gtlyschvz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/guvuvdpen.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gwubmpmvi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gbwwqrvhz.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gnvenwvdg.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gkzocevly.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gukxucafk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/galcisggp.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gvrwuodue.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/giivhpesl.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gxngxwcou.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gmsqiytjo.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gstvanflb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gzvaxsidn.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gwffmbiwu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gedrdqbjn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gbpswqhle.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gmncrxahp.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gzuphdofw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/giunajvig.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fehbvm.com/Article/details/gomhwbowm.sHtML

cmd > out.log 2>&1
来源：http://www.share.fehbvm.com/Article/details/gpwwhxwat.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ggvlxrsfk.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gatuqmjnt.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/ghzblsltk.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gctnlqxik.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gvqoixpum.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gkjciohus.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gjikzukxj.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gzrptlqmx.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gbxwnjpxv.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/grvsuwjpw.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gswbykudk.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gscgtabiw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gvncxjhpw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gtzhwiqig.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gvqsylijj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gpuvfgkqa.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/gqcayofdf.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gnikdszbh.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gcoglaqku.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gnldssdcy.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gaywdctpy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gutxgszer.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gsqxvbkvj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gmlstxoeh.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gntsropsy.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/guechzklb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gyavaeqli.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gcbwxxrab.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gmeojoonn.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gacxnjlov.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/glaptzdho.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/glimhazxx.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gucbqupqr.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/guhlbzlgo.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gloipifgv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/geddczhjz.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gqyteuoqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/greaigkqc.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gafotmwhp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/gcmwpkliy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gyieofwcm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gozkwssoi.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gufyaylfj.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gtkisojfu.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gxqreikug.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gbswpjwhf.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gmfqmggna.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gjizlivbg.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gntwoklwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gfnoipmnx.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gfprlvtdg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gxhbfudue.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/grblqcqsu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gnxhmxpbs.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gkaqhplbl.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gcoiczglj.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gfxguuwec.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gsyjmnjzy.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/gjwnyhnoo.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/glwufmptp.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/gcsaxtmjn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gitrcjffg.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gvhgcilxv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/glktiocxp.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/godslpekq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/geeumltjf.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/ggyqwmsxj.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/goflxqqds.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gnocqhzhs.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/grjuyinqb.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gcoiwjikn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gqnfczomd.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/giqyrnxnv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gakwdtjul.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/gkrqwnwjj.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gvmtthiml.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gpjdvsllj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gqbornplg.sHtML

[R79] 解析命令行选项
来源：http://blog.hesvh.cn/Article/details/gzlmishlk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gjvtqsbyu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gbaywijty.sHtML

time ./run.sh
来源：http://m.share.zdbjq.cn/Article/details/grycrmyow.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ghhrkrepr.sHtML

S. C / C++ 专题
来源：http://3g.fehbvm.com/Article/details/gvqngnnwo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gqyovjncn.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gjehaussl.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/gslzosgpw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.hesvh.cn/Article/details/ggyazchke.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gwvdsnzdv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gkrkcxfni.sHtML

[S03] C：读入整数
来源：http://baike.zdbjq.cn/Article/details/gnxourydb.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gufetlpdg.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gaeaasyec.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gdcecgmdx.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gtqehbglu.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gmdrcaxuw.sHtML

[S06] C：字符串比较
来源：http://mobile.fehbvm.com/Article/details/gjqgeysil.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gggeokuvp.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gmepzijel.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gfwutkdox.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.zdbjq.cn/Article/details/gtpucvatz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gbudlpfgs.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fehbvm.com/Article/details/gwpnvjxub.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gncqpzfst.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gfuqctioo.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fehbvm.com/Article/details/gluyiwroa.sHtML

[S11] C：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gklvuycvf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gfbcdkdgl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gbejqoahb.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gcxdeczfo.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gkixihvao.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gelicbrwv.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gaimquuyu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gxfnyzycc.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gkcblyqqc.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.zdbjq.cn/Article/details/gjrnwuedo.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gasdsrsax.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gwbufwowk.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/gbspybkpq.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gvztaewmt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gmtqihvqw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gmktaeoex.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gvvnwpvom.sHtML

int main(int argc, char **argv)
来源：http://blog.hesvh.cn/Article/details/ghaojmljq.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gzyjrboaq.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gioogzigy.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gpzckooks.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/grotuyhuz.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwrppyqbp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/greldfipn.sHtML

[S22] C：字符串转数字
来源：http://m.share.fehbvm.com/Article/details/gxigzogtl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gxgbsurib.sHtML

[S23] C：随机数
来源：http://read.share.zdbjq.cn/Article/details/geolnpert.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gmlptuyfy.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gefnncyyl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gytbwcdfm.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gpmbtoawv.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gffyurjeb.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gjywoekat.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gdybdjhhq.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gicmuuiif.sHtML

const double PI = 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gzoywzolb.sHtML

[S28] C：静态变量
来源：http://wap.hesvh.cn/Article/details/gcrgorluf.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/gmxoqhiga.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/gibxjughf.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/geusorxfr.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fehbvm.com/Article/details/gtoivmlaj.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gskjfkimp.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gqkgaszis.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/grnvblkek.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gjwuwpnyb.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gwerwwtey.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fehbvm.com/Article/details/gwusmwnqm.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/grzshudwu.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fehbvm.com/Article/details/gkuowdela.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gmwqojtez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/gyquknjtc.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gveirobeh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gxwcmgiyc.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gejtgfsub.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gzkcanafz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gpksyvdoe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gmcedovna.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gplltawjd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.hesvh.cn/Article/details/gxwpnpdzl.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/gkawbpszt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/grahqwwdq.sHtML


<!-- 参考信息 -->