代发 wailian999

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gcyavgntl.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvsgabocf.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gufeamral.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gbymllsis.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.fehbvm.com/Article/details/gipizqzpi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gjktdmnvq.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/ggycrgziq.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gcjrdynas.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gsjznzduc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/ghbbxmofx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvgxloztu.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gcbponvez.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gdjzqowaf.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gsnofepho.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gkkrncukk.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghkmorehy.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gdbpvlyig.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glpyagfhm.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/grakavpgw.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gtqtlpdcq.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/gnwqncaqa.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gbodqslct.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/ggsovlddk.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/ggshdfpjz.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gwojfbpyt.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gnzllcocw.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/ggxnqbvkl.sHtML

[R05] 参数默认值
来源：http://m.share.zdbjq.cn/Article/details/ggmfsvtam.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gwiggkwfr.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/gkahmfdar.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gzsmjphba.sHtML

[R07] if 判断文件
来源：http://mobile.zdbjq.cn/Article/details/ginkxbfgo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gsfmvczfq.sHtML

[R08] 数值比较
来源：http://www.share.hesvh.cn/Article/details/ggwhryrmf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gynrkqbri.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/giczevtjb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/gizuvltze.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gxmqokjcc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gzxwjithm.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gxukvwntc.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/glurrkwbu.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gjxblochk.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gwchwdgzr.sHtML

*)     echo "未知命令" ;;
来源：http://3g.zdbjq.cn/Article/details/gjuihvypl.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gfhnarwrk.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/ghtzhqfba.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gxeuohuba.sHtML

[R13] for 计数循环
来源：http://www.share.zdbjq.cn/Article/details/gkjtmnzsl.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gfenbcqbt.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gmkahlavn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gwbeuobva.sHtML

[R15] while 逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/giwxxbphp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.hesvh.cn/Article/details/gbmvpgpga.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gdvmluwhx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gaeloukzk.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gheadcliy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gwqdufsor.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/gnkevhkse.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gjfgopbeb.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gldartgpk.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gocbwzvlw.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.zdbjq.cn/Article/details/gkbupcurf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghhkedtbx.sHtML

[R21] 字符串长度
来源：http://blog.fehbvm.com/Article/details/gadjdqicx.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/ghfxsnood.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gtutyjzei.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/ggrfmeaik.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/glbqntxzf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/gmjwysaau.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gbsyhvgeg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.hesvh.cn/Article/details/gqozapwdm.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gefyrrdam.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/gnmxeqfkk.sHtML

[R26] 命令替换
来源：http://www.m.share.hesvh.cn/Article/details/gkdofcnon.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gamqichlo.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/grrogvbiv.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gytrvmzxz.sHtML

[R28] 浮点运算
来源：http://baike.fehbvm.com/Article/details/gbrcfhvmo.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gpsxpiutg.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gdrjrlbbj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/genkqjfbc.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gtmmnpeni.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/guwdmaswu.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gwwpxzzbh.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.zdbjq.cn/Article/details/gettrtpnk.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gkqmbqksv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gzbeffqyf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gjacrbkis.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gsjwihkng.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gylyujpng.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/ghjmpumlx.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/geapnlcua.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gsmzldnfr.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gtenbjgoh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/gspeomhzj.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gkeyzkyrp.sHtML

files=$(ls -1)
来源：http://www.blog.fehbvm.com/Article/details/goozlqgsb.sHtML

[R38] 管道串联
来源：http://www.share.hesvh.cn/Article/details/grbkelnqx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gfoywkoie.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gwveygmmz.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gnhnmyiuf.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gbspuoamh.sHtML

echo "log" >> out.log
来源：http://m.share.fehbvm.com/Article/details/goptwyejc.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gdlzmuebl.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gisrgijfv.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gzlsymbzi.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ghrpdsvkf.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gjsptwpqd.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gecwykout.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gqhjyjsfm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gzpeqlnou.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/grzjlvwyo.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gomkzfovy.sHtML

[R46] 递归替换文件内容
来源：http://3g.zdbjq.cn/Article/details/gwqypiqba.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gelxauigs.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gpefcxsee.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gvbkgnghk.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/gpymqylyb.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gajsdjnmr.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gzregebpn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gsmkcsglg.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/gwlorarlh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gopugrgnh.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gelmidybg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gtyhzjonv.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gggqbicgj.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/glyrqhddy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/guevzoduk.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gwewizwih.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/gtiwtvklz.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gohcdapsz.sHtML

[R55] 压缩与解压
来源：http://wap.fehbvm.com/Article/details/gliwxmfvw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gptubybko.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gpylvjuxu.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gfeedzgkd.sHtML

[R57] 远程执行命令
来源：http://www.blog.hesvh.cn/Article/details/giaaaddkp.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gkcsfwmqf.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gvjaiazxe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gwavbkmxt.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gwkemvxbf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gpevnahol.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gsgtdshgt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gfwvalzva.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gnhluqbpb.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gfeflxmhy.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gbzhntnko.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gsyxfgome.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gljdmvuhd.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/grcftcjfx.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gmmndhdft.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gkbhozbqy.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gmalfewhg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gmhfsjgzi.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/grctjddjg.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/gaeunwzte.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gflytokbb.sHtML

openssl rand -hex 16
来源：http://wap.zdbjq.cn/Article/details/gbiyxxgrq.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gxrzwswar.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gvvonzemc.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gdggzptxa.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gprnyxqdg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/grvughior.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gwbpotejj.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gnmbgxdag.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/ghdbbrjeq.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gbsxyrwcn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gptkqyfhn.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gikhqexxd.sHtML

split -l 1000 big.log part_
来源：http://3g.zdbjq.cn/Article/details/gafixtfis.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gmrajaait.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gzsgbnnqo.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gixdhmgci.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gwnqrfdlv.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gjynjjhuo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gvekgjajy.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gejrtgbbj.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/ggdjpgppk.sHtML

[R78] 交互式菜单
来源：http://baike.fehbvm.com/Article/details/grvyghdtx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gbiwdgpsx.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/grmkbbvxl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.hesvh.cn/Article/details/gscsasqsv.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/gdcboceur.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gofgtggjd.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gssovmuix.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/guxuriima.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gnxhmsryc.sHtML

[S01] C：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gpqhxnqnp.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/grzzdpens.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.zdbjq.cn/Article/details/gfyqjmbke.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gtjvfrmur.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fehbvm.com/Article/details/gshwoejwy.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gvufvygof.sHtML

int x; scanf("%d", &x);
来源：http://wap.zdbjq.cn/Article/details/gdadvyadu.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/goqearfwx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/ghxibqxig.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/goecuvohx.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gzafzzsvw.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/glbvqhzem.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/grxvmckve.sHtML

[S07] C：数组遍历求和
来源：http://wap.zdbjq.cn/Article/details/glnvdijmy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gcibvcmww.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/geietuoyp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/gpcpkjfxu.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gtfoxzvkq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gijxmhzty.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gllnrvukn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gxddkmcfr.sHtML

[S11] C：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gmlrqypkt.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/gkyeiaboh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/glpuobqiq.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gkwrsgvol.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gtkekceuh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gsakxxlbm.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gxbgmnzky.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gasubxtfh.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gixxmaxyk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gwqbqwaiq.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gkfwkhjib.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gefjabciu.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gyqkutlfo.sHtML

x |= (1 << 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gpshsitsk.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/ghrxhgblz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.zdbjq.cn/Article/details/gdinvmouz.sHtML

[S18] C：命令行参数
来源：http://m.share.hesvh.cn/Article/details/ggoiqmosk.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gkjkifoek.sHtML

[S19] C：快速排序
来源：http://www.share.hesvh.cn/Article/details/gkssiqvsr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gmhuigwsh.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gkbipjpce.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/goaouzbld.sHtML

[S21] C：字符类别判断
来源：http://www.blog.hesvh.cn/Article/details/gdgxcdqfr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gdnjkigjx.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gkjejrdmp.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gaxuyqqqx.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gxhoguqhf.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/galnzwxdn.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gmuasiqdr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gibpvyiqp.sHtML

[S25] C：内存拷贝
来源：http://wap.hesvh.cn/Article/details/gloexngxg.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gruncaeqm.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gdlowgoux.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gayxyovyq.sHtML

[S27] C：定义常量
来源：http://read.share.zdbjq.cn/Article/details/gxuagrlnh.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gbhhwlwjn.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gvudipvot.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gdncitruf.sHtML

[S29] C：变参函数
来源：http://m.share.zdbjq.cn/Article/details/gtrjxfpur.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/gzncrdets.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gsrozscmj.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gcamkewts.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gqfefgnac.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gjtgswqka.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gcwruszum.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gidfamvdm.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gqwlevhoc.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/gdvyggvso.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gixckcuez.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gwslsdjhz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gusvzpgnc.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gywabyctm.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gxmgthcyb.sHtML

[S35] C++：map
来源：http://blog.hesvh.cn/Article/details/gtaubtkvq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gjxapqhrz.sHtML

[S36] C++：unordered_map
来源：http://baike.fehbvm.com/Article/details/grvscamaa.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gwjjwacxz.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gsjzccbmd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gerbockqb.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gfxsntfsb.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/glrfjozap.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/generdphc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gyyjrwhkx.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gtvftyopa.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.zdbjq.cn/Article/details/geceumfwg.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gnstihglr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.hesvh.cn/Article/details/gvgmioxrc.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/girrhuzzx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/geceiirvj.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/guwmfnxjv.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gtkegaeyy.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gteidvdkx.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/ghxqaprkv.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gkrjjolhp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gltgrnfzp.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/gjlwdrqor.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gskwaguwm.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.hesvh.cn/Article/details/glmpcnpdj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gunmdzsog.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ghbmirnik.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gqxmopdch.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/ggddbdabj.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gvwdapalz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gizmzagus.sHtML

[S50] C++：格式化数字
来源：http://wap.fehbvm.com/Article/details/gothglkkj.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gwdhxvggn.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/ggpjtnepg.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/gsgsnuqpa.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/grzwxwusm.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/getcccngq.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gtucvqwyk.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/gsjgjquqr.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gijufglav.sHtML


<!-- 参考信息 -->