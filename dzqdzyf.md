代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/ginokrltj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guelvxqtn.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnwdrggk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giquyllso.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywiclmfu.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gzxrogyiy.sHtML

[Q85] 数值取整
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpkepfsp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fanxiaobao.xyz/Article/details/gdptjphiu.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gxiivtfgm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gabkucfhx.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfruenqsz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlfzaceb.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gnuhrwpgm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzindfda.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghxywljev.sHtML

[Q89] 判断表是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gkhpqrfml.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcjtdhlhv.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gvxuumvgw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlkigclk.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowiswies.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gbsndivjr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjcrrkye.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gzhmecamn.sHtML

#!/usr/bin/env bash
来源：http://www.share.fanxiaobao.xyz/Article/details/gexxkkeuu.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gqsjxwsdo.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gunsdgbot.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxvhylnm.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gfxlzxocj.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyfnprvy.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvqdboio.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gsjzbuwbr.sHtML

[R05] 参数默认值
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjyjbgxm.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gddbjoapz.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuxbynvf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gativigdw.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjyrjojb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdasajmro.sHtML

[R08] 数值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guzfsmcki.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gigsuubsk.sHtML

[R09] 字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcgqjzmeo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gbukongza.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gxncamghv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqnfikyxo.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gzbtdgmmy.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gixxrfplf.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gdxznardw.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gnvxwgwjm.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gumwzxddu.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gwrqytgqy.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghcqrwlyy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gigozlkto.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtfyyytdz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gitdiaoqe.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gvtbgmjtz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlzdacim.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaetqkahq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gintyiylt.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdbxquyg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjmnxkjhe.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gjsavdmfg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gttaytnuz.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/grmygmusu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgscobwn.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gwftgpjay.sHtML

echo "${#arr[@]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcjmybzzo.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnopxbgdw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gaennhmdg.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gynczydhd.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrqncwmk.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/grghkkkfs.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gaxfaktid.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/glbbybzsr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhnqkyft.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gzelxggzm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdljdgdey.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqlnerkh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqwifhdp.sHtML

[R26] 命令替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpxshqfc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gsvasazbd.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/glhenhpoh.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gukaclrxl.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/gnstwfwab.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/getdnrusj.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gublzubzr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gncnoqxzm.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gbeiuufcn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/gwqfrosxf.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gzjfxcwkw.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgmxfrxk.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gksbswzkd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjbzuejtd.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjhqetqup.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbtbnmqix.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/ggebdwlds.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpqilkro.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gykdfcgzf.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gpeiwcihl.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtapjdmzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gflyoplih.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giyznrdtz.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmfjhakq.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gsatlqgow.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gzuzruzzi.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gcldmpdbh.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gvbjskduw.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gapkihzzd.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxvnatib.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmzrhsrl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gliqrmlcr.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gvqocziye.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvshifkts.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/guntoxbsm.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gdmzntcjq.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gmhfzfpkb.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gtocevhae.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gabfklszn.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gawselcjv.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gajsskmdw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/garxonovd.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcwqaoxgu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkgkkxhtg.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcdkfynt.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhjgjwhd.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gyqhuhuqm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fanxiaobao.xyz/Article/details/gialfqhsk.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvaanticb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqgnrtaui.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/galscrlxs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gggjcbsdw.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghkdrxsbu.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfgncbpe.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gvxigyukz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fanxiaobao.xyz/Article/details/gfayxbfxn.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtxqiwxfp.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gjrspzxtn.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewkoldwc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdbapsbc.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhipatez.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gwfpwrkbb.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gvwbbwzea.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gtjebadsm.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqagsgnsg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gwadghdtj.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gjexdtths.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gokuzwqgg.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/goxrkobsq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gsimsaxid.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gprmflwzw.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmxvorai.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gheyvnlip.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gmegtraak.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtgmylliv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gxjwwzfrl.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwnxxkfj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcgpcyrrf.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gnncvgjbg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlaegime.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwxqkcgck.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgzsbzep.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gadylojor.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gsrzqsnjg.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkftiyjk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gforkbfjo.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdfwrdwd.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gveozzhwy.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/guvrvyxnk.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehqeirvm.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gtqofmthv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/geygbezlb.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbehxssdi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtiknblsz.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gqgfujxbz.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gjvxbgjoy.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gwegsloqi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gytjstpxl.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjibzihqi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkjrvaks.sHtML

[R76] 使用临时文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbkqzxbkn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gdoumvhsa.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/genhktufb.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/grivilbzz.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxaogndw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpkkhbime.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdsqehqr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gwurksucn.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gqwlidhpc.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyiwytlp.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/goflhdijp.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvvgjhlo.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/ghggqcypf.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwobnagg.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbrnlpbq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fanxiaobao.xyz/Article/details/goeynpxly.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gxrwtmlfb.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbirufrt.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gabnxajmu.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzosfxokw.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgfmjaep.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gwxgycboh.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/ggmdgpgop.sHtML

strlen(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffqftcfj.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gavgfdenh.sHtML

strcmp(a, b) == 0
来源：http://baike.fanxiaobao.xyz/Article/details/gptsbkgfm.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gadqpfhgd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbxryjdy.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/ghlwxxwkg.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gerpmbjmy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gpoeeiqiw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fanxiaobao.xyz/Article/details/gpilzvqho.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/giazzgjcd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gswxqrexo.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggajxetgu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fanxiaobao.xyz/Article/details/gfbmkqevc.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbcvgkgj.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gvbvwoqkn.sHtML

[S12] C：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbapftzz.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszvzvusw.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gdowmbujo.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gotyjklvh.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/grsefptvv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gihisbdku.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkdpolbb.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gdhbqcdjj.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gclggwmms.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guistegja.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaorztxo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/ghldfngql.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gxddbqmmn.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeanjvqv.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gbbtcioko.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssjyoexi.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gogbgqprh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqljhcpnm.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gejjhgbra.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/giqvbmmxu.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gnibdyqke.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvbmwdnz.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjttbnmk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/grxtanjtz.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gbfbameuq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchsvikky.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gymvudcvg.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjcffycqd.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgkgwiif.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoerfamt.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gwocjyaqg.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gtxzwgeti.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtzsshrgi.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gceprsudh.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gclacnopy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgefeeft.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gsatcxmau.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/grmpskmxm.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/glssjthvb.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gveoeoloh.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlghiofr.sHtML

#include <iostream>
来源：http://3g.fanxiaobao.xyz/Article/details/gaugkwmzb.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgbqxetd.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/geouqevxr.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkpzzuzth.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/grqqhcret.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gpndeqedh.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/ginybtsbu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpjqdloqi.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gojhhnvku.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxboflsv.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gcnpobwpx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihmppqjl.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/genkjuhkv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gunumciue.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gvumdfwhz.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/grhnyjang.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztlvsskz.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gzyozybcf.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gzvzfomqa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gvdxybubc.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/gqqsjtulh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/grldiezfj.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gvswpvavm.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/grvjqodjk.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzskwhfo.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzavysztl.sHtML

[S44] C++：引用传参
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxcahstsw.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guwqemmil.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gbzkylnau.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/glhxsjhpi.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gxklmrxvm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gytswjkyh.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/grzfphagf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbmcwoesf.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmvvwbgrm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gqtcfyvle.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/ghaujljin.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqkpwzfai.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fanxiaobao.xyz/Article/details/gkthspcyc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhbmqzfc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvzmkkcw.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gumniqwiw.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/giunamdse.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gvzishhms.sHtML


<!-- 参考信息 -->