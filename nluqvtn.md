代发 wailian999

[Q78] 当前时间
来源：http://3g.fanxiaobao.xyz/Article/details/gjabkfsux.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/ggmrzxypb.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gorvsygre.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/grctgvbzg.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/guxwhkquc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzergkvu.sHtML

[Q81] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gxgtiztbg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/ggiiwskyj.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gdegfzioo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhpfusot.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganrnacbl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsflbmpdv.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gobubragy.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gwaosmfvh.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gkgklpndh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gzeytkiug.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fanxiaobao.xyz/Article/details/gnardqvhp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbplfjox.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gecjatryn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/goaywmdyr.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaqvsekm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtybobxkp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gctikmzqm.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gcziktvmb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gdpcspyks.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gnzprnpzc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgrxtioc.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gimupuwpn.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggapbszam.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gvcqilwwr.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/ggeljxnmx.sHtML

#!/usr/bin/env bash
来源：http://m.share.fanxiaobao.xyz/Article/details/gcliojflm.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaawfgojq.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gpbetvlmo.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggumepkzv.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gysoxbbms.sHtML

readonly PI=3.14
来源：http://3g.fanxiaobao.xyz/Article/details/gyhbiswce.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gxpurxjus.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxkjcavn.sHtML

[R05] 参数默认值
来源：http://read.share.fanxiaobao.xyz/Article/details/gwegeyucq.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfwndthr.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gsoheoors.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtuwfalid.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gszhdslhz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyjjplmzg.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gongiowwf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ggotudzuq.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gxghjymua.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gkysaeobk.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/glhltongf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gwkszwdsk.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gbiqgqszn.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/ghczwxghq.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnfkkhnj.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gexwpjknc.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gexegwqez.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/grlndjdri.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gidflxjvx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdoaiccba.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilqmwehy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gluhflxxy.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gzucozybl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgmfizae.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gftegkndy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozffchth.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gurjwpgep.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gobttclmo.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpnwylkn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvvocvwd.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gmueegbcv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gssvvscbx.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gseeqgjag.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzehgloi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtihleize.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdwnhojjl.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnzerebl.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkujybue.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gxwsbbfgy.sHtML

echo "${s:0:5}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtrsglytf.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gtlujhuil.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gtldhmtvc.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhlgnnkt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gakfpcmnz.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/ggxbjucpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzjzakuo.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjitgbde.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpbilgbid.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/gihkgmotx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gsieuwjml.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gvtpbuzzk.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/ghizlbedo.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilrqgckk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fanxiaobao.xyz/Article/details/gpemnuxzi.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gmnqwjjrs.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/ganqaozlz.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/gpkzwwmrn.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gfftqkgvc.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gtvvkjqtt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnhwsmzsr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gkjrrwotp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gtntxfeph.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gkjsmvdsr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gyorbqmcq.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gaymejhon.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gbeusqhti.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiquwcta.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gzjncrimz.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbjvetpqt.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gnxmydjgx.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcyaetns.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gdiyhoons.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gwilnbczk.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gspfkbwzq.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gcopisgip.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnalkvua.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gijcoemkc.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzvvibomz.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gygsnyhvc.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvblyhngt.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gangboejz.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gzhubbdsl.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gnpxrxzla.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdcschzvf.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/geryzzyhq.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxeyroao.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/guwliumpv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslsntmiy.sHtML

[R47] sed 单行替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfasiloh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggdqnzglg.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/ghhsdcnjg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrkliqzs.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaqigdqs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkmsdjpe.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilywablv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gazozenud.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gfesvrtax.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gomolisxf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gwnljblei.sHtML

wc -l a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcigiwcwu.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwerjlvj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gudhodstv.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/govzqgliz.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gaohaotzi.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwneyrwb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gujpduvnj.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrxknsti.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gbnbfpeqq.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeomtzrf.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gxqivrkwq.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyhbvwpp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/glzdyxsbp.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gxablvrss.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbykveys.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gusaxtgyc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/glcnljjtq.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhuimyal.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhppcxxi.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfezeryrg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfpvtbaku.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/glyblclin.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/guznttdis.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyavpjoy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzvnxdgx.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxilniezd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gabsswaio.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/glsnmhjwg.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gfsnkdcdi.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ghhndvzhz.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gzxuovoyk.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/goaoxsrwa.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwezzelg.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gijdxqlni.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gzgkpvqnb.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/gyloanxjm.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fanxiaobao.xyz/Article/details/guopcnwdv.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gevfsctla.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdldeiftc.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gueireebh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvxytejo.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gkweawbxb.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldrvyspv.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gntfjfkyg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geysytagm.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gwhdfjnvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxacfphts.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gejnaujde.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifktwzfg.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gprgjljde.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxywlqlhn.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmzfnspuo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghqsfpyya.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gwcmfnrgr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvdkiyfpr.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/glxfohvhj.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosthskds.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmddyynda.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gbfrhifzn.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfcfgmbzr.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gvwdahqxs.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gwzsojmyj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqhvooyka.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/guepaxqjr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/ggigsfymv.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsevungep.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gphybbpsq.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoecfzib.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glepuhnpb.sHtML

[S05] C：字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gzddktwhq.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/guugqlbbu.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guucxkbng.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gdxchwkgy.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuefpavv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gwcnnrltl.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gprfymtrh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gfokxdumx.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/guqnomamf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgcuyytv.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiznerez.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gfbwbxpgb.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsoabuoqz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gqasaylpk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoglriyd.sHtML

fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpcrklmi.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaascyrgt.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmspnmmka.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvbwczia.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxrxekxsy.sHtML

[S14] C：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbowtili.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gfpoglhbw.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ggeswakgv.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gcmlfkfpd.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/glubglcmz.sHtML

x |= (1 << 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvgneriv.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gaenzctri.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gjfctirmm.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyfagqufc.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsfbgcpoa.sHtML

[S19] C：快速排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gislolyzn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbbfxqpm.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gmbruvafh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gllcznthn.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpkskdal.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggryhvhff.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gbwqthnoa.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiepolio.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxkqwhwp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gkbfqbhnv.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gaafcdppo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwivvfil.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/geuwpoakm.sHtML

memcpy(dst, src, n);
来源：http://mobile.fanxiaobao.xyz/Article/details/guvmrvnae.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbcehnus.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvwfjqkqe.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/grgjkxmzw.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gntdhoxkf.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gckpbaqbe.sHtML

static int counter = 0;
来源：http://www.share.fanxiaobao.xyz/Article/details/gdejjtgjm.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gvodzlwzy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gxbolaltl.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gaipvmzyh.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gfcxatrxw.sHtML

#define X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzgcnqyv.sHtML

#endif
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmkfctoc.sHtML

[S31] C++：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gkdztbgci.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gavqmwzgc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuvbjvyc.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoygnojd.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftrefuwp.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gczeassqu.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbqmsfwjq.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gcqmkblcg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gkwdaaxns.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gecdtujyw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijdsijjq.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gamidwsgi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gddzefnzd.sHtML

[S37] C++：set
来源：http://baike.fanxiaobao.xyz/Article/details/gqvvqjcgb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gwqddrtcc.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gamiorjbx.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwugdpby.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmaqomohe.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gtwumznol.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqxblqvvz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnmnozgc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtntvmhq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnqnwlpe.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhqvgzgf.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gstccpkfl.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/gstwzxmnm.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/garsigtqr.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsrfsksp.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmphewqal.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gcomtvhps.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gltfhsyjg.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gbrstmaui.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpucbotpf.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gurvirubd.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwzfwfrj.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gummrohns.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/guwcynvoa.sHtML


<!-- 参考信息 -->