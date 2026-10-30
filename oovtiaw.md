代发 wailian999

SHOW INDEX FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcobsifh.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgerjhic.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukttcpom.sHtML

[Q74] 强制使用索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gpykmuopl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnirmnvvl.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gmeuiseoq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkbecpbj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggsnqyzwc.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gqokvvbne.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbrewzup.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmspdhlt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fanxiaobao.xyz/Article/details/gxxtfhfff.sHtML

[Q78] 当前时间
来源：http://www.share.fanxiaobao.xyz/Article/details/giamricvv.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gqjajjnvp.sHtML

[Q79] 字符串拼接
来源：http://mobile.fanxiaobao.xyz/Article/details/gkybphufg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvlvipse.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhrkjtey.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhrkslnz.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcoximmmt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/goplqjeee.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnjfnchxd.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ghzrlxyam.sHtML

[Q83] 大小写转换
来源：http://blog.fanxiaobao.xyz/Article/details/gdlfrilub.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlbwxryh.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/giudawalr.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzleqoop.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gqzxdepte.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhkblget.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpslhpgcq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fanxiaobao.xyz/Article/details/gjtcqhnma.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fanxiaobao.xyz/Article/details/gzszsplxe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gemorkmfn.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfskkacas.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fanxiaobao.xyz/Article/details/gvbbhflnw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuenboks.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gnihjqwjm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbehvgtxq.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkhhkcuxt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnjpaecu.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gytzobagn.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ghftpqoeu.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxffivpkm.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/goncnnlxj.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gqadgqeft.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gvscwvvoo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gyryrlmgp.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gnxppynmf.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gohhuuhhp.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/ggenbgdcz.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gycttqrdt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fanxiaobao.xyz/Article/details/gojshtfqt.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/guwxobnko.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giubguyfk.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdhpgljzw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkteobnat.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gswgoeynv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzrzcfjp.sHtML

[R08] 数值比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgsuqjga.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gxmwaddbi.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gtdotlpld.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuyemiky.sHtML

[R10] 正则匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjimuwbt.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gaifmaqfu.sHtML

[R11] case 多分支
来源：http://baike.fanxiaobao.xyz/Article/details/ggxncffds.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/gutptktrf.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtalbhpbq.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gggeaueji.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqvqxcjv.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjdxgmoy.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsbdldqz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gamxsehcy.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gakjlgbet.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gixkpywzf.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gfhhshaol.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gekflmmvu.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjxxwdfb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsitxvic.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gfdxhwocx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gtmqojfgb.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ghjncyhrw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvdiwuscf.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gfjsdbqss.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghllvuicx.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpeyispf.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjovwjwx.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwsuqczw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glnyfjzvv.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gupevbpbq.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxmbqthj.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/galqxmkmp.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxautmdts.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbzuvrmb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fanxiaobao.xyz/Article/details/gkbinudsd.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/giipquwyt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gusyrsrnv.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gihpxbpfx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqrmxoim.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gduhxtsfg.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/geenivani.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gdvbsuyhf.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gbizmfnqy.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpxllwyz.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbjwjqhu.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtiphsaxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwznmfso.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/grdhpunjv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsxlqxqj.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gtccbanst.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grpyminsw.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gwwwpupji.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gahtdctqf.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofnktnbt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/ggavpqvjy.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gjiopxpxl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gbloxawau.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gngxbnjoe.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibdffkbd.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzenjmtp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gazsdmdnq.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gortmlgvf.sHtML

files=$(ls -1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gygbhtqjf.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/grixoddfu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gbswbsdpm.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fanxiaobao.xyz/Article/details/gvkhcvwbn.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gzdmabbgu.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcttiqnvn.sHtML

echo "log" >> out.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmpjtqfl.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggevqagdx.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnttrxtxe.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gfjivbdtc.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwzfhjmi.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glakroeav.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbonyyht.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gpefkrdvu.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozbbuhtp.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gtlrdtfyx.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdgdldre.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmtemwdl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/geldvggaw.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gowgrapyt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/glxzxjuyi.sHtML

[R48] awk 取指定列
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgssrjhe.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpensiti.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gvxpamhwm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gxotsufcl.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/giswnldqn.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgcbcmr.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gzofijsxb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gtjlgvfug.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gjqtwdvam.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gwylfqkns.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fanxiaobao.xyz/Article/details/gggzpjwgh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesxbfozg.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyzrnomlp.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxuvslmz.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gafsrcyek.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gnavvqpud.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gzdsfisvn.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqyspjwj.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gwznngjcy.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gsjxxubiv.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gedauvkcx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfqtdrxe.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gczsjcixp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhjbmdwk.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqczsstc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlnhgyfy.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gtnguemul.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgpactyb.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gavehyzzi.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnoqyvajm.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gylfyecza.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fanxiaobao.xyz/Article/details/gludxhpzd.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gzvbgpixa.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucwupyck.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoffvgwg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gjamnifyv.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwonviosb.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/glijxnpii.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyvtyqhl.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgrgiuzo.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/grqvhqtwj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gifskrpei.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgpcbneo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gckkxdkfw.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/grevbbiea.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxkumezy.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gypkoylnt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gikdudycy.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gdtfzlrfa.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdrjccimv.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gfvvmydho.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajiuwdbp.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gvpyljerf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxdmanovy.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/giwwmrfim.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gvzrzurrm.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmlxayqkm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/guajpdtnx.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gbblscvtm.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/glrouadna.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/geqbtrnii.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzsodewds.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gulcvtesm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgppctyd.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gabfycttg.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/gcaqjmihd.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbqoupom.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gamuqfrdj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gixhthnfw.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbwjyqos.sHtML

#include <stdio.h>
来源：http://wap.fanxiaobao.xyz/Article/details/gqqloglef.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gechwhtsp.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gpdsqcena.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gmiawkzlh.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gnasuccbb.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/guhsfgcni.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gypulmuxm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/ganiadcua.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/godyoobqd.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnksuncpb.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfaiodnc.sHtML

strcmp(a, b) == 0
来源：http://mobile.fanxiaobao.xyz/Article/details/giuonjfps.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/ghxqpdgst.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gfbiznmup.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gpadptiis.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpzzyquil.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gfwcvlnpn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/goexvdwdl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzijgklc.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fanxiaobao.xyz/Article/details/gewawslig.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzzlqnuc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtyxxlij.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnqellxhv.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkyesbrpt.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/glsnzvpcr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gldmqafnc.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gfclhfeqh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/gdymnkvbs.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqzvxjsj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/ghczctkxu.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/ghagxrsyb.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gaaizhfvh.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gptjofltq.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghikeofyu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gzpbetadp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjugkaav.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvjnhckj.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/gyhofxfpv.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gmutebuhs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gdgcczbbn.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdtdrccx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gaqdsuosd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghsyrneai.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/grjscpbgl.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/guevdehdp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gdpxxkpdz.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gikewapow.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/goqelcgxk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnpqydya.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqmndtdy.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gddhfjzsc.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/ghfctgpgd.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gatfsgsdj.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlicbevh.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabhfzfjv.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbyikrmg.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkewrkwy.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gvxygmcff.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/giwclrbkm.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/giidisfos.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkdounne.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gbvafykpt.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/grhgcacmj.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gsqsylois.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grejnzogr.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gglpetvms.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjmjrpqp.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gvxkucnbt.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdhbiwia.sHtML

[S33] C++：vector 增删
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxwbgtpj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gjbngrbky.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gogblgope.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhrkqalh.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gasmgnwni.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaavxdwft.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhlzyvaf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqounwre.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gqszkdpsb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/grpzigoev.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gfoyluoiy.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fanxiaobao.xyz/Article/details/gxysbsucp.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/geifwjlfl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkyaldxhd.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlkiagsx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjgpcrwh.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjupnkia.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkuvmyfl.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/glpsxlueg.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gjcibhitn.sHtML


<!-- 参考信息 -->