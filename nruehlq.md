代发 wailian999

ANALYZE TABLE users;
来源：http://wap.fanxiaobao.xyz/Article/details/gjjpctruq.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gzjrgjnia.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/geescknbs.sHtML

[Q72] 查看索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gubxfaszy.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsewuggpi.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkjlrijq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuykobwr.sHtML

[Q74] 强制使用索引
来源：http://wap.fanxiaobao.xyz/Article/details/gxswvylew.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfxdfyjz.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvlzujrf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gycgfgkxw.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmkcivpz.sHtML

[Q76] 按天统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozyjxabk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcoooztlb.sHtML

[Q77] 时间加减
来源：http://3g.fanxiaobao.xyz/Article/details/gyrklhcam.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfnnxbbr.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/grnokkspx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxedhwft.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gikrsgqcl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpovkiby.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gtznmsoot.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvwgdsdh.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/glzdyfpui.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gvnkijqez.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsvynzmae.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfznexum.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbixkxtmb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxaxtzrsu.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/grvatmwrw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnqaqqxou.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gvikverho.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gdbwikcmd.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.fanxiaobao.xyz/Article/details/gwgtpwcft.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gujmjkcrp.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gfbwyfdvt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/glcsyjhrj.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gobrkkowp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjnnbtel.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gewypbjzw.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhhnhdij.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmakuwpn.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ghbrjrzqu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giofdopxv.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvlekjsim.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gvbfmnqsv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/germyrwsk.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndblkdit.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbruqtbos.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyhlawkp.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsxqzcpg.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/gmplpxgga.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdvqhqnq.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppwcdjkz.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gqoouwxea.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrghgwge.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiywkxws.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaomowqs.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gpemzjjwh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gecrspsio.sHtML

[R07] if 判断文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvezkrqww.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gszrqffml.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfjdhhrp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gycsnewby.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnukocsz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/giyrdgmgc.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gisjanvzz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgzveqzg.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/glwmldyxr.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/grfxfhvoo.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gneeavqim.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqqhydocq.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbhbymkj.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gcjrvhida.sHtML

[R12] for 遍历文件
来源：http://3g.fanxiaobao.xyz/Article/details/gozvspgrs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjmqnuapi.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ghyjhxial.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoowwfbl.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gaggpcelo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaqkasyc.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdkceyhbw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgcwdhfu.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/guvhrdgax.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxyjtmfvu.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gqixthtua.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwmfhshe.sHtML

[R18] 遍历数组
来源：http://baike.fanxiaobao.xyz/Article/details/gkphppatx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwweciqme.sHtML

[R19] 数组长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gycmickbq.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfhwukcl.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gppujofqb.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gypgqxxkl.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gtczpnaiv.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gplturlmp.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gopvydtiw.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsygxgbln.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gfzumlxyx.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgssfucr.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gpihaydcl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvuguiwbo.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/grdpejwpu.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gloxnvqyp.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gucellnfq.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyfdpwkz.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/ggxkrmmri.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gsowsobxn.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoznmeqb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gtucdysac.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/goudfynju.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxvkxikyx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwgkcxpo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gdivamacp.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmnalhef.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykjqschp.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/girodybkr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqmmtrkhu.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/grljduvpu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gigfbtytp.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoufmnfb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gjfuyqrzu.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvpuefjd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmwtrvtlp.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gudtpckdi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqyjcmsm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjbwzrdx.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gpyuvqhku.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/giejfkgsh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghhjbpsbk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gupyeofkh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyjqetls.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhuqgtwo.sHtML

echo "log" >> out.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmuchpmgu.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gqonnxngw.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gairmgoeh.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/grntkscik.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gajgpehag.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gagduaflb.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/greofrkme.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpjzdeyg.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gikwboelf.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gorvrwiwe.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsecdjxk.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gygjboibk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gscnzjxxr.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gtbmxefyo.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gunpudgti.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/giwanjyhy.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwajvnle.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpmgehze.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gazafgkdk.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gzfgyihpx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gztjzanbi.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/ggorghnak.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpffqnfud.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxsexnsm.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/govfcqmkv.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/guiumtzmq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/glrtdhfny.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gidbqiwfe.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glltqinmy.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkixeykx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/grwohgxcv.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gzokymuhc.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gioqccczt.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcqgrlyx.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gjidoynjc.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gbvajrqvt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzhctdno.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gjxxywrik.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gctiwbrdf.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnbxqsma.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gpewergmz.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gttqwzyyz.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gytzekzyy.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gcjdbicfu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnrdbyoh.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxqqkvgv.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqxuicne.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grjkpnsnv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvjohlxs.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gqrblokwn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gqryhakmv.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gaypuossq.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfvqehhvg.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfkuhpgy.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/glowppsnd.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gfidzlgjf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsjaynanh.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/ggliafcis.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gtnuafppy.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/govnjpuuu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gdkfvapko.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gdocbnvkp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gpetpuoxb.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/galddhhrb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpqcjhisx.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gdfjrynqy.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gghjvvwrl.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gkrdhmfxo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gscevecxk.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcjvfbvg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/glkwqplwd.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrmrncgo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gcbnficpq.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/guvwqgehv.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjysnsyb.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gbbexjvjn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsftylfmy.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gbnkmpxsl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/givxonpyu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gcbitsnig.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gpgrxwpah.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjupobcfw.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gimzfoejn.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhzplcbx.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gwocfmzha.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkdcngdi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfudtacb.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gnnrxaktc.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmywssofj.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrwokprf.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gijnvtovh.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvoldrzm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchvgfbac.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gejxwzunz.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupthvmq.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtqfjsoqu.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gzorbgilu.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfxhfbuk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gowwbrzql.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgncepab.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gatajpycg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gzbzaftss.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkytxogoa.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gfortmszd.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/geqcpnqnu.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gbehqrzne.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gphpfvrpy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblzhalgv.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsfydzyw.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebrqmbtj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxdrdmnt.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gwpmonjmf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gcokvviis.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpzlubji.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjzbbpxa.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gtgcwqxkc.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gwfkktxrw.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gzqlxavgh.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gotilotzr.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gvtpeqmty.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgmkrdvn.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gouqmkmhl.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkljoayf.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/guubkfjyx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gyqnfbgej.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/gxhrwkmse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyudcdhqq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/glvnjdjfy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gorcaucbb.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemqffbic.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmaxkkhbj.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gonptluhz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gkiclqhbf.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gqahrrzhl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxauthunt.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldjnpcvm.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/ggumxrsla.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgdkdigr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gzdxgodzm.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gqzlnqqqr.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gktjvnakd.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gzihhnyhv.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gbbkrowab.sHtML

[S29] C：变参函数
来源：http://blog.fanxiaobao.xyz/Article/details/gnqffilkz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gpborvkqj.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyzkichxd.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gniaxnflt.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbbrsmrv.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/golnngzlb.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gvbdlxhud.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gcsuzgmhj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqtwdttrz.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gyxjqtksx.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gttuoqofz.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/glulcqmle.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvopxaaly.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/glczqviiw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gccrmzzgv.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnuihuqo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzqpqlvf.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtlxfllw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaluyolp.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gimvixupf.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrwboxcv.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gyutqpoyb.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gajwmbcdt.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxlibdcy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/ggdpszyef.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnbxvujf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylqyqnnu.sHtML


<!-- 参考信息 -->