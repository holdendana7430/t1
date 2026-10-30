代发 wailian999

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gxmfviuro.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gnisoyeqd.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlosenzi.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gndnhqmmi.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gobpkjnrr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fanxiaobao.xyz/Article/details/gosallnmo.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gywwubjgh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjppabig.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/graztjznp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvfdxwkn.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gokhvzkdc.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwbczjceb.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdfmravf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gcqctbliz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocjmqntl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrpnzddp.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gjlbaqdrm.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gueubmnxk.sHtML

[Q85] 数值取整
来源：http://www.share.fanxiaobao.xyz/Article/details/gjglwlizy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gyumxqemd.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/ggpznagcf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/grqxbnpcl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszxjvakn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtjoasxfu.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gdljyfswk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giojfmquk.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqcljbhuk.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikexvomh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpeexjve.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gnffbxuje.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwoyzyaua.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkfwlnwcg.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gzjamoovd.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gligdfrft.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpssazsgl.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/grebzjple.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/glwjcklhi.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/ggcmolxbg.sHtML

name="Tom"; echo "$name"
来源：http://wap.fanxiaobao.xyz/Article/details/ggpheqdfs.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxzeyejj.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gfxwrxstp.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/gmskyjfvk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxorqipd.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gpdjrcbqr.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvffpdjxy.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grjtrubxl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjifxlrq.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gelclwugx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gjtdlmrww.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gcwyqywcg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gqqpbehez.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghpkreujn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpxtxomq.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvdltooo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gjbnbtaoo.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtsfplzlb.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gkrckzsbx.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwuotzsbj.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtvknawy.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/geflkivlw.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdjxzcyc.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwcignwkv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpaltslmm.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gniyokplr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gygvdtzek.sHtML

[R14] C 风格 for
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgetjotr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxeiwctq.sHtML

[R15] while 逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gjignyxwz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/guudqnsww.sHtML

[R16] until 等待条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrcbrnwt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gtnagwure.sHtML

[R17] 数组定义与取值
来源：http://www.share.fanxiaobao.xyz/Article/details/gayhaxrrt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjphhyrb.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gugujebyz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcmbcwfc.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gaxrxkqzj.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gamgunrto.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlowfivj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gdgpikgzo.sHtML

[R21] 字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghahsgryg.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gaxtqlsga.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/ggwxdigve.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gogfpqqyu.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzunkhfsi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gkhcjwcjl.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gyepyvwlg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkiziroge.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcxixjpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gakemalaw.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxbkmrex.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gbmsqegpa.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwujqgvk.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaplsbvy.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzebwmxu.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gsciyoean.sHtML

[R29] 定义函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrwwdbxq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwiirzqdt.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gizbialbj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxpfzper.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gmmnrqrmw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbbkwfbu.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtanldpi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmechkfig.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gvenavvzy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjmlkcbaf.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgxpoxkq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmwcrevve.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/grywnjyvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdolqnpus.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gtihfscjc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gbrhvjwtu.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwhnpcchb.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghgcchym.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszqqvolg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fanxiaobao.xyz/Article/details/gpvcvitrh.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fanxiaobao.xyz/Article/details/glusdthtp.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/glomzkzqc.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/ggftdbppl.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gagdvyxcb.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gcaibhvva.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmgedxnw.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gyuvsrnqb.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnslhvhdy.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyajjlvht.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gkmlcmuqu.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmpezuzrf.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucjvllih.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/ghbsfeusn.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gyztqirlt.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gwjcaycag.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gtncfsjcr.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gsxkjasld.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcojnloaf.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gghyixtrq.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnidcwdkq.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpamrwkq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gijtdukmn.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gudsnnqnj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/guvepfnic.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gmgcbalcc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyoxmynu.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfncugiud.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsyrzylf.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gxsmtiilf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjpiozkw.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gikevjoau.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhsysexh.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/gggwotgrs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gtxmcsfdr.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gfxbwopvz.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gkkfjthez.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaybvexp.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxxhwojg.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/griqboapk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gcxiciuhv.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gijufcdnu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxmwwaoda.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/ggeqfmuis.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/guoibhbww.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gwbznxhnw.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/givbcrscv.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gurkdndar.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmwkjuwx.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gqmareahb.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gvebdilcw.sHtML

[R64] 结束进程
来源：http://blog.fanxiaobao.xyz/Article/details/gxfsjxvsq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/grryawoon.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gfjgedtct.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gksuewavo.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gckexfuou.sHtML

crontab -e;  crontab -l
来源：http://blog.fanxiaobao.xyz/Article/details/gcafjxoaz.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gtgtsfdzm.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gezykihbo.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gufmhcknx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giaqrmlob.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gwhncvxkp.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/ghakioxek.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gpeamiwsu.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjriggqq.sHtML

[R71] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/guxgyrxmz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gtzvpycfi.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/glibszkno.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gxratukjc.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/geoilnyty.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/ggakigixq.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiiuleas.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gkeytzluv.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gwrbfkbdr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/govjhkfpx.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfwaftesa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gkqmidobd.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjlggbfa.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gzxfzilii.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gvtbnynig.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbrfbbwf.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gkylogacx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkzykdopz.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwyvjdfq.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gyguayaoy.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqvejwpjh.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibzpaxep.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gklxwdzfv.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxyvkymp.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghegssypq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaumpqkr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gwuqtlngd.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fanxiaobao.xyz/Article/details/gmuegtpjf.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvpdwbli.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzchfikfy.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghnzxrksb.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gvzvybpud.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqwiozxzz.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyldhdesp.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gxasxfpbn.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlatfjpq.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gtljyuskg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwilqcvu.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfdxanrz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhsoczuz.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gvuhmapfx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gaizezaqj.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getvmyetn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvvsexzeo.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gxxtbxtgl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gughikgsn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwqsuftq.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gwmbxnwsd.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcrcvkyw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnghfchvg.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gosopkomb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fanxiaobao.xyz/Article/details/gkylpxult.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbljqcpr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gpudlylpk.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gysxoqcix.sHtML

(double) a / b
来源：http://www.share.fanxiaobao.xyz/Article/details/gnemcsfsr.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/ggnytqeqd.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/ggeqcbxch.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gjthkwpcr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/glbrlwepd.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpxgfbsgl.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlieukww.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gdffxpgqc.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjrccjlav.sHtML

[S20] C：二分查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtlkrfrct.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gnzpfpvhw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukhlrlvt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.fanxiaobao.xyz/Article/details/gwpdgtenk.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdgcnhrkr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbtictod.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gxspsuicu.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gxlgfihdx.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gvycihwpr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/goxtysbuz.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gauxruzyu.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gdnxwojml.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gjveqwdgs.sHtML

memset(a, 0, sizeof a);
来源：http://wap.fanxiaobao.xyz/Article/details/gsfjtqkbe.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnsmkhqc.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gshggjfxy.sHtML

[S28] C：静态变量
来源：http://baike.fanxiaobao.xyz/Article/details/gnjksyqxx.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkfrucqw.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gdfuhnqbo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpjbdkwx.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gtzhbygeo.sHtML

#ifndef X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gaevvsxry.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwwkuvmt.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvnwueqe.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmlhgavu.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzadiowxo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyqhylxb.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gibscievx.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fanxiaobao.xyz/Article/details/gcknxnpse.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/grsstjspj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwarxznfb.sHtML

[S34] C++：遍历 vector
来源：http://m.share.fanxiaobao.xyz/Article/details/gdivjiatn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggujbfwdy.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/ghocpieyy.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtthlzxfn.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyypwmci.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/glbfeoaao.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gpgwauiwg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gqsapqgih.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gegwsfmkd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gantgdena.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gptpcdxzf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdofskuzv.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/goyijwlhc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkwfatfv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gedrzsfab.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gweezwnxz.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gwetxthiy.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gmfcawwzw.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjcjbvss.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gepsoustn.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfinvsrw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqttyixfl.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/gdzseohyn.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtpcblbe.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gleuwgvdk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvhetljup.sHtML


<!-- 参考信息 -->