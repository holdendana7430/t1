代发 wailian999

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gmsijejov.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gdnrslksk.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gujzbvika.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gacgmuvwp.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.hesvh.cn/Article/details/gjezegklm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gvovikpal.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gyctzlsxx.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gphdmkluv.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gmffzyuwb.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grxozskgm.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gdorcscsx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gemgonjlb.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gczpybwqy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gjvauovbh.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gwknoeqdm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gscugrvmh.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gowroebwb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fehbvm.com/Article/details/guekzbtnz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/grutlqxtt.sHtML

[Q89] 判断表是否存在
来源：http://wap.fehbvm.com/Article/details/gdiluxvhs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gmkchfvwa.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/gpwzjchtd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gtsbwrbem.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gisodnwnt.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gdedqysus.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/glfluwzjo.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/gktzpheuk.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gaxqqkjhn.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gldxnbtvt.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gwwecprev.sHtML

name="Tom"; echo "$name"
来源：http://baike.zdbjq.cn/Article/details/gedaxzbnv.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gjhwbdait.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gjfcmyoox.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/glbcxtchb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gqmvoounc.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/ggdwduxrv.sHtML

name="${1:-default}"
来源：http://3g.fehbvm.com/Article/details/giynnqsyl.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gpkqkfnwy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/ggnlybvvd.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gdzfafres.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gvhauvxbt.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gezjpyhgr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gglbismgi.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gmfwdntki.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gmyeykqpt.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gnlldjjlp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.hesvh.cn/Article/details/gvjjuyqlk.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/ggcklelpi.sHtML

case "$1" in
来源：http://baike.zdbjq.cn/Article/details/gbnxistyy.sHtML

start) echo "启动" ;;
来源：http://blog.zdbjq.cn/Article/details/gfkyywvay.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/ggcptwspc.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gmcuewmjl.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gmtlfscoc.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gfojcejtp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gyqyvgghn.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gqsygrkxs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gppadoiqo.sHtML

[R14] C 风格 for
来源：http://mobile.hesvh.cn/Article/details/gyktjwxhv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gdedxsakq.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwnrcpkoj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gsalkbxlx.sHtML

[R16] until 等待条件
来源：http://m.share.hesvh.cn/Article/details/gyzndedcf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gjljyrgsr.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gaxsjxzlt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gsfyqsyua.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/ghvpoahwt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/grypvcfwf.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gjmzdpyab.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/ghjlnwudw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/ggyjgdifl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.fehbvm.com/Article/details/gwiauubxb.sHtML

[R21] 字符串长度
来源：http://read.share.hesvh.cn/Article/details/gieqlokqa.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gtnotzcwo.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gixpgvuht.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gsvhnefqh.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gifacruyc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gdsompcdo.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/gwfkgumiq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/govrmxsgk.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gvsmuumxv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gebequloq.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gcoljpxlr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gwowqkfil.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gbvxpxzey.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gdkgfuymz.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/ggrhwjwzg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gkucotqjp.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gltrdmmyx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/ggrhyaugk.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gycsxlgnx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gdzuyqdho.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gibyivtpq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gzzgtxnii.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gvfqhewqx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gtjngijjb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gpihmwyru.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/glejuksya.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gzsoxmftz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gqiemwupe.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gmfachhar.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gjyupqjpi.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gbboydezq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gjvuneuca.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/grklkranw.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gzvrurvpd.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gngutazvy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/ghcwjszer.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/giaudecll.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gwqcettdt.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gadlnsefz.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gqcweqnbb.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gpxiibpbx.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gnhiahyqi.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/grmstjvnn.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gpdsuffei.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gilkngvbt.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gpphqyyxv.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gpuydznmo.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gezntkeju.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gupfwawrs.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/gxlseftcu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gthqzysro.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gxsyfhrax.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gkooengsg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gvwlofzcl.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gmnmlrpnv.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fehbvm.com/Article/details/glintwnbv.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gmzpawgav.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/ghsecqsup.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gjlgebegu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gdukhktfo.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gwuumxtbz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/golyouhfr.sHtML

[R52] 统计行数
来源：http://www.blog.zdbjq.cn/Article/details/gwcwrjpvn.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gwmmakzhb.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gxmrvniwv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gbbqivvgt.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/glqtepycc.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gkrawpjlx.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/gabrtwado.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.zdbjq.cn/Article/details/gztozkmjk.sHtML

[R56] 远程拷贝
来源：http://www.blog.hesvh.cn/Article/details/gxuobapat.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gjifmmygr.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gzmlbdfif.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/gawyxneuc.sHtML

[R58] 下载文件
来源：http://mobile.zdbjq.cn/Article/details/gnkgrrkfk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.zdbjq.cn/Article/details/gtdamwnkr.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/giruojfip.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gkuezesbt.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gzfnzhnpt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gvpxgscit.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gzmywvqyf.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gjyxzpduu.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gnemhnvut.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gaaalxbol.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gitlrkmfg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gndowpnrw.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/ghbrftzmt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gqojpfjdz.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gewvakwce.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gvtarpnbo.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gghzcjnqq.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gevfpwglc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gglufetjq.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gpomgbclf.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gzqnslrhm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/ghaqymmug.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gehcuojst.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gvhfzrwma.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gvkdeqcao.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/ghbbokgkr.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gvuiezdcn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gmecnrvxs.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gsrcfqxmd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gaofaomvq.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gxutdfdgd.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gaiuuwnva.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/giykrsnhm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/glhxaogfo.sHtML

[R75] 导出环境变量
来源：http://read.share.fehbvm.com/Article/details/gpmwwqzyj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gwrouldvh.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gpkxcwgck.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gmpsvxylj.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gkztzzrkt.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gdvtzjcng.sHtML

[R78] 交互式菜单
来源：http://www.share.fehbvm.com/Article/details/gztwehhuk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gbmmqqhdf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gzdzcibto.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gdetyijdq.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fehbvm.com/Article/details/gldpajtqc.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/ggvmvhsqz.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/geemjvofn.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gihwdipms.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcegvnqdd.sHtML

[S01] C：Hello World
来源：http://wap.hesvh.cn/Article/details/grlyfkcxt.sHtML

#include <stdio.h>
来源：http://www.m.share.fehbvm.com/Article/details/gdnkheffj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gykxxifbi.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gudhdoyzo.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gydffdadu.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gdwtrknij.sHtML

int x; scanf("%d", &x);
来源：http://m.share.hesvh.cn/Article/details/gkppprgnl.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gjcyhgjxj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/ghdfjiwts.sHtML

[S05] C：字符串长度
来源：http://www.blog.hesvh.cn/Article/details/gsaereqno.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghazknumz.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gomhfexfn.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gxxjdanbi.sHtML

[S07] C：数组遍历求和
来源：http://3g.hesvh.cn/Article/details/gwbphwowc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gbronjjtn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/gbobqfckz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fehbvm.com/Article/details/gqfqihhvp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/guhcthyqd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/ghkfxcbfu.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gdhmvaizi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gfmhuxofx.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gpaesopns.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gxgwrlbqm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/gllplyeeq.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gwiqdlost.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gwbpeytqq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gcaxyrcgu.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gctvizikk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gvunppoth.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gpynuwcwx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gspouvuyt.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gvxjhytfz.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/glplpqoax.sHtML

[S16] C：位操作置位
来源：http://blog.hesvh.cn/Article/details/guaqpgwis.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/gcwxbnofw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gbosrzeuy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gohannkxs.sHtML

[S18] C：命令行参数
来源：http://mobile.hesvh.cn/Article/details/gtcfeojdl.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gtodqqves.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/grlzjbgdy.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gtiqmcbmk.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gbxwkmfef.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gahfkrdyq.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gzjwxicia.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gglaikfki.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gzjeeqawc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/ggllvkndr.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/ggtyfxayj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gegdyejma.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/grnjqygoi.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.zdbjq.cn/Article/details/gocqjeuyf.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gdgtyzhoj.sHtML

memcpy(dst, src, n);
来源：http://read.share.fehbvm.com/Article/details/gadcxkvca.sHtML

[S26] C：内存清零
来源：http://baike.hesvh.cn/Article/details/gfstymadw.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gjyhniito.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gatlkfywy.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gejzthaml.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gmzqybjjf.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/goixrsdah.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gatgyqgfa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/guldmwcbk.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/goftlsnmt.sHtML

#ifndef X_H
来源：http://www.m.share.fehbvm.com/Article/details/gsmlftmzp.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/goitxgdxs.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/ggpjgqure.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gsbkjfjvo.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gafacaouv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.zdbjq.cn/Article/details/gcubcrgrr.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gcbpxszst.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.zdbjq.cn/Article/details/gjvdbvruh.sHtML

[S33] C++：vector 增删
来源：http://read.share.hesvh.cn/Article/details/gwswpnxqd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gguacurtj.sHtML

[S34] C++：遍历 vector
来源：http://blog.fehbvm.com/Article/details/gnziqlrjp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://blog.zdbjq.cn/Article/details/gfcysandj.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/ggsntgmvr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gqxvgeefy.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gtqqmvgal.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gzudvmqqb.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/gbciagnff.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gwidkurqb.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gjtrortas.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gykhazmzl.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gxdaymbju.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.zdbjq.cn/Article/details/gnwzpjspb.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gjbaglryu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fehbvm.com/Article/details/gcpyoldjz.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gmonfklmz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gjpohnejg.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gmtaclesm.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.zdbjq.cn/Article/details/gopuvwiqh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fehbvm.com/Article/details/ggxwdnwms.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.fehbvm.com/Article/details/gevlhumcy.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/guowrylhr.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gipqicqxy.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gjrtiddor.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fehbvm.com/Article/details/glpzmtodu.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gbwtgqhbg.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gxfvvtfbu.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gachmmioc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gljmdltkz.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gfpaabezh.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.hesvh.cn/Article/details/gjupdhryc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gmyqnqibe.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/gkkkqssuy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.hesvh.cn/Article/details/gyzxdjbvr.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gsrrwnfwr.sHtML


<!-- 参考信息 -->