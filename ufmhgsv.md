代发 wailian999

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gdxzpeuuw.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gaortarun.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gasdafoda.sHtML

[Q70] 更新统计信息
来源：http://m.share.fanxiaobao.xyz/Article/details/gediiuqev.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmmeqldq.sHtML

[Q71] 查看建表语句
来源：http://wap.fanxiaobao.xyz/Article/details/gkwwdqfja.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilzumfkr.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gtiplfcns.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqprqqlor.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgwgsbfz.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhevzwzz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvzsvigr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gilztzhnm.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gkhfnwcoa.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhlxewlt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fanxiaobao.xyz/Article/details/grcuvgojf.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhffyoxv.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzoijrczj.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gyzqylusv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmbwsoks.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgxikcxu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gwzgemowr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcwvjgfx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gzukhhmzt.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmfijspk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gdohqyhzh.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsvqejhqw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/graqusbpn.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gniewepsj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gqtuyvekx.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gedgkwyvs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjsycwfon.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gskylzsyn.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsskgxzy.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gvpilhqys.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gybwfysvi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqbdaxfe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gqxfgaceg.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfevpoybi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gghnxgqsw.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/geigqpkwk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gwuelqfva.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grtdcjjet.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gjttspwil.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwzjzxvt.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcabfwljv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/ggptpzzku.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gnonirqfi.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gvitkbneg.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwekvxyus.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fanxiaobao.xyz/Article/details/gebhaamzt.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gubssqafd.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gestjaifk.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnqejmmgc.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gukmapopv.sHtML

[R03] 只读变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gskljlgit.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gifpnjzab.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/grogsayqj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjubyltw.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprmbccqb.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gokjutmpp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gjfqurotk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grhnwxjmk.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjvxhaja.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gxczukyhv.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuhsgsoh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkxfajaz.sHtML

[R09] 字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvzlklxu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gcykgukgh.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gcstyqzlu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gicpwntwf.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyodjgvvf.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkghhusos.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxlniqvlr.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/grsissebi.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gzephzibn.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gkfhxgrzz.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gsdxfdhvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gyoytqdfl.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejcasfki.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppnyspar.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumyvjltc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggvrnnlwx.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcaojcyb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnpzortf.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvkyczwl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcbhjjnx.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnobswhv.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgattrps.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gqcmarerr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcdcpahob.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiuzebyg.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfkbkvgn.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gbglsioeu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glwlotbkw.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtcvcqvj.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gopjyxymj.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwnmbqlr.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/glroirxhc.sHtML

[R23] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbjseigbk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbdefikmr.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpwautjd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gpiaygmqh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/guanyulty.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkeuyjmoy.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbasaqhw.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gvpckiqbs.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gqgbndqht.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfitlovo.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gichahsjc.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gulaqgylv.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guthfqvih.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gymyzoxfd.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gmvaupkln.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnyzhxscg.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gaejehrhz.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giphvczby.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxloulap.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvozyubrz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxdabkhd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzwozqpd.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gzkevnmsv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvbcypzf.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwoxtaqy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzkpakieg.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gzgxrcdwe.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fanxiaobao.xyz/Article/details/gguwpoctf.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gomxxppyp.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnudggjr.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzzpxrqzj.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gtyprsivh.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gveezjqdb.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gurdkafsc.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gybsurrdp.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gimflpdsf.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzfuepto.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gizchjnkf.sHtML

[R42] 输入重定向
来源：http://www.share.fanxiaobao.xyz/Article/details/ghandbgte.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtuiibmvg.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfrewwbfu.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gepcvgbdk.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gukakzeay.sHtML

find . -mtime -7 -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gsyuvaxxs.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gijvoihss.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfhttnfr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gckorrflv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gksbgafay.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhgcqxnp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzciswtq.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gggxpswis.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxchbggr.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gecxwcdrs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gvcbpucho.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggbcfxwwn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ghajqzddm.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gyvnaansp.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gppcchjjf.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gyezafgvs.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/golowhysc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrjzoncp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/grucjbgka.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gflihonjt.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gojciwqpk.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gmodnobha.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnkbyqia.sHtML

[R56] 远程拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfbmflhvn.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gfnzcoiwl.sHtML

[R57] 远程执行命令
来源：http://read.share.fanxiaobao.xyz/Article/details/giytmeivg.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ggsmqaiui.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gopmflbkx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/groricyhe.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/glpgbgbxk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/goplnoeis.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gktjjmltv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gljxhwbvi.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtyruplt.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeobdybk.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghqltmaid.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbqqsssm.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/ggptslllq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gruyxcyph.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gysbovfqk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gdecwajbs.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrunjywd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcrbvnpx.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnmxxvuoc.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhqwinvk.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzolrgad.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidlibtxh.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gpshficla.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsvevdyk.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnblfzhr.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxjjjnzb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/guylhruve.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glojgafqw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycjdxmnh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gzcpdbspo.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzvofapj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwzubddh.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gytpoehuf.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gzjyqnmgp.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/ggznsurhw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gybmwulxa.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gousxdaov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpkvulpdy.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gesmzwlgo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gyaejmfit.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gtagewpup.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/goeqnynwp.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gadelmkpu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfyqfbzkq.sHtML

[R79] 解析命令行选项
来源：http://3g.fanxiaobao.xyz/Article/details/gbecytbpl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwlipmelr.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahzgevba.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxdbhokf.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxsvrahax.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghthwsgms.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/giryzolcu.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgwoaqba.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gylhzrsgx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfzgzhnk.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjgkxpixb.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gufslnozf.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gghstgnjp.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gbkmrbxjf.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gupjfltbx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gosntibys.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gqtimxjfn.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyyzyaftd.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaxriwyg.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gqotvqbfp.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gtsqwdska.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxabbzqs.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/ghpjlyoye.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gxthmtibb.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwydhhnsq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gybyxuoms.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gutfcujjb.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gjmyxkbhz.sHtML

[S11] C：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghxelhqfd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gambhboiw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnmlxars.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjbzsxpz.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gglfepaho.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geogzcgtb.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/grseamgrs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gwifrkbpw.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gebpagcas.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/ganjgwmzj.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gniukgwfx.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpqxjvio.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/ghsvzlrmq.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzamzyjkc.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/ghydaadun.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gnotetbne.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gcjqmxpdi.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzktoqzyh.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/grrynqfpl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggjpaxjto.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxflfctn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfndpqvt.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gelhioayf.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnghgrdn.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gucptkxyi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/glfwmubqs.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsueakfyl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gqhldbktp.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gupeeknuf.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpphexwgw.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gteqezhgc.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpowbwxmo.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gupboawqt.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwumpfwln.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gxtsgkxml.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/geoujmcnl.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/gyozqznzg.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzhblrxp.sHtML

[S29] C：变参函数
来源：http://3g.fanxiaobao.xyz/Article/details/gmabjpxrt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gpxhqcwwf.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhkzqtwa.sHtML

#ifndef X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gijwgtxfw.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfstwofgt.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/glnxxdldo.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/ggloyddxm.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gifrqjrwm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gsgisqpju.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjhaaosgz.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gunzyzqrb.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gykcxkiwi.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gujdacjzf.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gwazdrtqd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gaujewqny.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gxoikfryn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaltctgx.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gvigtepjx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gvrufmjub.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gbuboaspy.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkieuiwxj.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkdrbxirh.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gqmpoqdhd.sHtML


<!-- 参考信息 -->