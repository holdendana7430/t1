代发 wailian999

[Q88] 行转列（条件聚合）
来源：http://read.share.fanxiaobao.xyz/Article/details/gizlzgjru.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/glencsujd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzuauxsa.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcqbkzxrw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffglbqlh.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaghobgsu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gtfomgdrt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjodndafc.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrhpxjzk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbyrmsuv.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gdhorbfcv.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gbhhgiqyq.sHtML

set -euo pipefail
来源：http://blog.fanxiaobao.xyz/Article/details/ggvjkwzec.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/gxppupipn.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/grwrygxly.sHtML

[R03] 只读变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkitmcki.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdgrfcdh.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtxqppyzt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/goseevzuo.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gncilidjc.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdbyjtpk.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gohjaisqf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrekftng.sHtML

[R07] if 判断文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfihetmnv.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghoqzgjjt.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gehxjlfwd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoqdkqhq.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjlghndx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gvrxrkhsx.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gscflqhaf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqhpehvs.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/ghkxgkmfd.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/ggyfcgyhb.sHtML

start) echo "启动" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzeeebkno.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkmrmmpf.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhktbtgo.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/grttdpwpa.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxwnkhhab.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glvvbxfsc.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/girhwmaam.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwpugvpr.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gwkkpwaou.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcinxldkt.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxoohhjuv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotdmvmbo.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/givjtobps.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gpmmhfbor.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gusduicbd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlmjvgss.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/gdfpwtjii.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnkvftlyr.sHtML

[R19] 数组长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijkuheju.sHtML

echo "${#arr[@]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/giplqzjap.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gfxemzsag.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyeiqltay.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbxmddgj.sHtML

echo "${#s}"
来源：http://baike.fanxiaobao.xyz/Article/details/gupokohww.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkjixtpp.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grjbwkgqg.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdlehavcg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeoyxwgn.sHtML

[R24] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gcsccbben.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxfohrylp.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuiogtmp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnztgfsx.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/ggzgayklf.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwcztyra.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gfhixjglx.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgptkwju.sHtML

[R28] 浮点运算
来源：http://3g.fanxiaobao.xyz/Article/details/gixeszumn.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/gxwqjmtmd.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/grhyrtqpp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/ghojxttce.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gbphgpjsv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gylilabiy.sHtML

[R31] 局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwetslogo.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gglzkuahz.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/ggwsszlyk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gblygupol.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrqxrgtr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gxvygqryw.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gndsqvdcx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gxxzohlfe.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gnpunrcrg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gtfipcgiv.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/gcikusfii.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gmznbfvai.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoguiylz.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbotydsm.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gzunjcgta.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnrdpevy.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqhiryrl.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gsmbbnsli.sHtML

[R40] 追加写日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gohqrfszq.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gulcfpwze.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gepdzsmww.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxeacgxk.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gqjtngttf.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gvhuyxsim.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvfgvqqna.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gybpjvoxy.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gatfnlsef.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqjivbr.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgznfioo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gcemspgdf.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxdlvjwc.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/grptjvips.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzqfwgrc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbvlwlyib.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/grilpkxac.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/goqehovib.sHtML

[R49] awk 带条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/groltwoyv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggcwvicrj.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grfgfcrkm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqhelvjut.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvchojquv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgmstpii.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmicqysmw.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gobmoqbch.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gmpcpwaon.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtdoideg.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gdwfbgftq.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gklpxsqqr.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmkescdq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fanxiaobao.xyz/Article/details/gfxtpbeyg.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gyzarcfuq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gbvydniar.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpnmswju.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/giflircks.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqdemhlqj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gqldxhfov.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gboibuhmi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/goagmjndt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfjmzsoa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gwldbkddo.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtpgowmpl.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gkmyatjwr.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhfhlskq.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gyficeqdx.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/grswrwlvq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/guwrnfkac.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gazqxntgx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcbwvztz.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gbxiyphpq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gxguufhoy.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/glxehmokq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbglsnuz.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/goxmilnoe.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhwkautu.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/grzmnaczy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbcsqedz.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqsdqqqe.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvavibwjv.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gouokiyhp.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqjsjajg.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/geuzmrzvy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/grcutrgxq.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gigcdfdgj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gkfrunpsv.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gyfctgavf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgnagxbr.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/ghpiplreu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ghxgdqgzs.sHtML

[R75] 导出环境变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjowhlpc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gthkkjmvf.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gccueaaia.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gyjpyezcy.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gitkalist.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gkqqoeeld.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gheetqouh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gggapjhfg.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gscjaifra.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtdjosrwt.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gxovvaalk.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjflzaduh.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvgcfygi.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gavzgksxj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gcdulmuup.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gysmzwzlo.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gparqyyib.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fanxiaobao.xyz/Article/details/gumtqdvnb.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gysunjfnm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfihraelx.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkrkqqsw.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbghioav.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsrzlalhi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmgmwmzi.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsimazfsb.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ghrvyxgkm.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgogytdt.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gwfvtmszm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gmejqufjk.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gqpniszvf.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fanxiaobao.xyz/Article/details/gqxtfstct.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.fanxiaobao.xyz/Article/details/gqothavak.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/ggbjiksva.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwbylztte.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gafjjahbf.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gjzaxobxt.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/grrabfqej.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkxebdis.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbhhiwit.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gouybpyvx.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghskezvio.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gnwqoddcj.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gekdwecri.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/grfeogklu.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gktevaidk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdeorjqug.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gspqweynw.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwgftsjr.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/gmeptpqnf.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/goqcyhkjz.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gribrdgib.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fanxiaobao.xyz/Article/details/glhralipu.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gocpmpsxg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdjxwgtg.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gvbvcztld.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fanxiaobao.xyz/Article/details/gikjnzxes.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gzrnysyxr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxwduqto.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/ggqpkyxbt.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkffdyyfo.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gdckzgvzv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gxbzmzgzj.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrzqlzgl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaggmqkcu.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gcalmhoop.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrtwjuha.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gyagbqjpk.sHtML

memcpy(dst, src, n);
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqyadaxe.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/gwhqgycxf.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gltmafsnq.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyrimemg.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/grxhgnrgl.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbqqmrby.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsrobyvt.sHtML

[S29] C：变参函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcccsaqo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gohnxsgkr.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmxzlzij.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gcvwpfwzt.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gauofzdmj.sHtML

#endif
来源：http://www.blog.fanxiaobao.xyz/Article/details/gimbabvzy.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gixjcsgkh.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gjlxayegx.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gapqhixrs.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhhfahnd.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/govrootbk.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gyzqoiubc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gztyjlrfo.sHtML

[S34] C++：遍历 vector
来源：http://3g.fanxiaobao.xyz/Article/details/ggzmcvqtn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gezauxvgg.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqiqwqfrv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkznowhw.sHtML

[S36] C++：unordered_map
来源：http://3g.fanxiaobao.xyz/Article/details/gdikniaga.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnfrzjjhl.sHtML

[S37] C++：set
来源：http://blog.fanxiaobao.xyz/Article/details/gcazthneo.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/geehebqyy.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkxudakq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrqffugf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyilotzv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gwtyxobrh.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpuhsoqem.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpcrzpdaw.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gguwsibqa.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gvlprnfhu.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnvqiipo.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fanxiaobao.xyz/Article/details/gvklgtfmw.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gfutqzmfq.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsnoibqsy.sHtML

[S44] C++：引用传参
来源：http://www.share.fanxiaobao.xyz/Article/details/gcppephqw.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcqlpcvwo.sHtML

[S45] C++：lambda
来源：http://3g.fanxiaobao.xyz/Article/details/grefawwva.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnufumjc.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gkwvteubl.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gnogmtyop.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfjopajk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.fanxiaobao.xyz/Article/details/grzabxjjw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxzbaauy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjvlacfc.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gspdylnlk.sHtML

[S49] C++：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gpxprjmag.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/godhebkem.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gjidwsctf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ghiirziea.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gticpypta.sHtML

static_cast<double>(a) / b
来源：http://3g.fanxiaobao.xyz/Article/details/geteekctf.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbfyaycl.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbviugxs.sHtML

[S53] C++：移动语义
来源：http://blog.fanxiaobao.xyz/Article/details/gwqasidyj.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaheuzdj.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvsmvtzb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyvbrrrm.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/ggxdtfrnh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/ginaxhemu.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxgqejsm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwngkdcgy.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gvbctylws.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsusckhnp.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gcuoszcuy.sHtML


<!-- 参考信息 -->