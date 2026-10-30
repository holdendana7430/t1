代发 wailian999

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/guuekayrf.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gslgynskh.sHtML

[Q85] 数值取整
来源：http://m.share.zdbjq.cn/Article/details/glpwycgay.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gxglevcpu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/grqdltljc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gsacqsfif.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gdvmdkgfa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gfjatquok.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gmnxvxcuq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/guupfedjc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.hesvh.cn/Article/details/gevrurczt.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gvmxqltpd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gwjavlfzo.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/glkrbcfrv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gwvpryxld.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ggyowsfuk.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gowtvwtfo.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geenaubvl.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gcedubbzv.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gnxwfsqpw.sHtML

set -euo pipefail
来源：http://www.m.share.fehbvm.com/Article/details/gwrzfbfqi.sHtML

[R02] 变量赋值与使用
来源：http://m.share.hesvh.cn/Article/details/gxqkzasny.sHtML

name="Tom"; echo "$name"
来源：http://baike.hesvh.cn/Article/details/ggwwjwlab.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gkbxqzbzf.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/golqkdsfp.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/giqtgtmsz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gngvendnp.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gukvektgd.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gebhphinz.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gmmnrjuyl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/guvobavyq.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gamcogrxt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fehbvm.com/Article/details/gcqapedqz.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gznyulnfj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/gwsakkamz.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gxyogvafc.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.hesvh.cn/Article/details/glqoeqfqf.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/grykaocaa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gkqvpduhs.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gftdvhfcg.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/ghwmtcxlk.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gnqzahcaz.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gmpkhopui.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gduitkthc.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gdphdknpq.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gqnlzvyxw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/glsgifzfz.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gexoqhjrz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/giidaddkn.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/garalbmbx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gfhoetunc.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gsyfxbjec.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fehbvm.com/Article/details/gjvxbizyx.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gehpvrapa.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gevcgblef.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gifwjfqnt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/ginxifjur.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gyrhyinqn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gnypatjdc.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gorwzkfrq.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gtjpvkbrt.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/goiepytrc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gcdfxnqvy.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gubfuhizf.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gahxhanpv.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gebozxzui.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gpwffimmc.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gacrkhfcf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.zdbjq.cn/Article/details/ggkkmruyl.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gnyssiunt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gbaotkvof.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gytkvchuw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gpoejvmxu.sHtML

[R26] 命令替换
来源：http://www.share.hesvh.cn/Article/details/gzrrtemhv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gspupvlgy.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gwdchqacs.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gouwhzmjn.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gfmqxluar.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gfmeqzhwh.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gxdpoictj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gglmizsfn.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/guqoxydqr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gwjzslchy.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/glynmakwk.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/grrcchgfa.sHtML

[R32] 参数个数校验
来源：http://mobile.zdbjq.cn/Article/details/gpifyuncv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gswcrvlkz.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gzzfjottq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gonipjoza.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gpotpkumj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gqwdbnqfi.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gidyyuayj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/ghvukyknd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gbpokygvf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.hesvh.cn/Article/details/grlfixauv.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gtkhiwahv.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gthnezdzm.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gzlxanbfz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gfrwsuxth.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gugxhypbf.sHtML

cmd > out.log 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gjabzzrdt.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gfqkequwd.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/glfdpvupa.sHtML

[R41] 丢弃输出
来源：http://wap.zdbjq.cn/Article/details/gvbmedloo.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/ggwadxthl.sHtML

[R42] 输入重定向
来源：http://blog.hesvh.cn/Article/details/gigwwamvq.sHtML

wc -l < a.txt
来源：http://wap.hesvh.cn/Article/details/gbbxalror.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/govmfyyaf.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gakyhywgp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gwtxwgwuj.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/gvjnixehn.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/giexekxku.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.hesvh.cn/Article/details/gvqldaega.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gysnmzqbl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gtpgrzkte.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gzzaxntwh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/ghkqfkrwe.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gpatqmkxa.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gfnvhdnnm.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gzbsmwmts.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gjkikptyt.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/glyedbkuh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gwlrtmwif.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fehbvm.com/Article/details/gjzmdszfm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/ginuwocex.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gbrhvutst.sHtML

wc -l a.txt
来源：http://baike.fehbvm.com/Article/details/gjcdfrsta.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fehbvm.com/Article/details/gahnqnzph.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/glzgpzwxu.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/ggiftoedx.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gjhprkyid.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gptqkgzrh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fehbvm.com/Article/details/gsnkidjjm.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/gyoouyyig.sHtML

scp file user@host:/path/
来源：http://mobile.fehbvm.com/Article/details/gbavvygsh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gcuajliyi.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gwvsgbgzn.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gdujlnsgx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gajpzzesp.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gpfxnkfsu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gvpkdnjbg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gxhyalmdj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gfezxshdr.sHtML

[R61] 磁盘占用
来源：http://mobile.zdbjq.cn/Article/details/gwbribjhy.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gqjivsjsr.sHtML

[R62] 找最占空间的文件
来源：http://mobile.zdbjq.cn/Article/details/givrinhxe.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.hesvh.cn/Article/details/gqhfrfoxk.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gcapbxzwm.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gspugatft.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/ggfvtafoz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/ghgzmpvpk.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gejpluffi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/grrkruxjb.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gxeddnmwk.sHtML

crontab -e;  crontab -l
来源：http://blog.zdbjq.cn/Article/details/gltoumzzq.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gtniqkgzh.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gasceoxyh.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gwiitgdmr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gfuumielp.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gnozxdznk.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gehwkwodz.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gfujnmvun.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gafiqedoi.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/grrycobli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gxatjtafx.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gpdfwrmvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gfbwyjlon.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gbduulmut.sHtML

split -l 1000 big.log part_
来源：http://3g.hesvh.cn/Article/details/gaihraimx.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gaxlzkhzc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gkwtwtjlp.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gldhcsszf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gsmqxgimh.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/ghhkitykx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gbntqzlfb.sHtML

[R77] 读取用户输入
来源：http://3g.hesvh.cn/Article/details/gmpridwik.sHtML

read -rp "请输入: " ans
来源：http://read.share.zdbjq.cn/Article/details/gbtbdszps.sHtML

[R78] 交互式菜单
来源：http://baike.hesvh.cn/Article/details/gncguwtfw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/gqfoknkrc.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gmnjgkvjx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/guallkjos.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/gpnxfabvc.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gwiijtwfq.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glnvzbjgc.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gqurqtnnr.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyoyvfvcq.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gbzuqxdbo.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/ghcmtpfrk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/gsfzshrzy.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/giqqugogg.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gkspuvlec.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gycbrpppi.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/gkibgtjgh.sHtML

[S04] C：字符串复制
来源：http://mobile.zdbjq.cn/Article/details/gkexvjohn.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gwxvkwcxa.sHtML

[S05] C：字符串长度
来源：http://read.share.zdbjq.cn/Article/details/gjduwthyh.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gbxcmoeww.sHtML

[S06] C：字符串比较
来源：http://baike.zdbjq.cn/Article/details/guofncdyw.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/grdtplqif.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gavmwowlr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.zdbjq.cn/Article/details/gseegzyor.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/gfmnojsun.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.hesvh.cn/Article/details/gaetmmytk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.hesvh.cn/Article/details/gzrcgjonj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gdblowofe.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.hesvh.cn/Article/details/gkygwfvkm.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fehbvm.com/Article/details/gndiuidvb.sHtML

[S11] C：逐行读文件
来源：http://www.blog.hesvh.cn/Article/details/gndwantfr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gimhedhhy.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fehbvm.com/Article/details/gpfqjdumy.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gmfhrorrc.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gejezopmr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.hesvh.cn/Article/details/gltrdpwfq.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gfwicoghp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gxwlebepe.sHtML

[S14] C：枚举
来源：http://www.m.share.zdbjq.cn/Article/details/gcecywwyk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.hesvh.cn/Article/details/gaptrakvi.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gsyejwhnw.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gdgsyvain.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gfrvjwisv.sHtML

x |= (1 << 3);
来源：http://www.m.share.hesvh.cn/Article/details/gznfnffhc.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gihlbvfxj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fehbvm.com/Article/details/gtnapblrp.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gxztokomb.sHtML

int main(int argc, char **argv)
来源：http://m.share.fehbvm.com/Article/details/gsctvopax.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gezcqbbjo.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/guhkfcqcj.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gomeyfilk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/ghwwnwlzb.sHtML

[S21] C：字符类别判断
来源：http://www.share.fehbvm.com/Article/details/gcajcinhe.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gauobdjiu.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gwldwxrbv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/goiywjbio.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gttatypaw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gddhqmwct.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gbkhsxkcg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gjhzriuqj.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gtijfdoow.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gpchldoaz.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/graarwvlv.sHtML

memset(a, 0, sizeof a);
来源：http://blog.zdbjq.cn/Article/details/guigcdsti.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/glzoglosx.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gihzaumpg.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gcvzwsqxk.sHtML

static int counter = 0;
来源：http://read.share.zdbjq.cn/Article/details/gphcovxwb.sHtML

[S29] C：变参函数
来源：http://blog.hesvh.cn/Article/details/geasnjzxl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.hesvh.cn/Article/details/gfpdrcxck.sHtML

[S30] C：头文件保护
来源：http://wap.hesvh.cn/Article/details/gpbmrtaez.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/ghtjqlzun.sHtML

#define X_H
来源：http://wap.zdbjq.cn/Article/details/goyhkligh.sHtML

#endif
来源：http://wap.fehbvm.com/Article/details/gjmpyccfu.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gygmagrve.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gdaqxmfvo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gjabwrkpl.sHtML

[S32] C++：字符串
来源：http://www.share.hesvh.cn/Article/details/gywexahvg.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/grgfhzljl.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/gcfgcwwrs.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/gxdgvhuzm.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gkgqrggjn.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gygxygipf.sHtML

[S35] C++：map
来源：http://read.share.fehbvm.com/Article/details/gomwwqmom.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gmdzhezng.sHtML

[S36] C++：unordered_map
来源：http://baike.zdbjq.cn/Article/details/gkvtclvkw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gmfygmreg.sHtML

[S37] C++：set
来源：http://www.blog.fehbvm.com/Article/details/guoylaupe.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.hesvh.cn/Article/details/gdmrpylyc.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gfxohekju.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gchwxruol.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gpwamdxql.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.zdbjq.cn/Article/details/gduaucvzo.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gajmjscje.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gikptlphl.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fehbvm.com/Article/details/gatobfily.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fehbvm.com/Article/details/gnxgitliv.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gyxxjqtsl.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gkfjsiwjb.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gphaapmzr.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.hesvh.cn/Article/details/gcptfxdto.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/gvtoiavik.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gmcgptwgn.sHtML

[S45] C++：lambda
来源：http://wap.hesvh.cn/Article/details/ghmgthesq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.hesvh.cn/Article/details/gqpbtrqhu.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/grkmfurls.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gmtswejox.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gjgomizdo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/grvzqtucu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gfxctzmng.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fehbvm.com/Article/details/gkfbzyglz.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gmejdldfo.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gjjojbeju.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gvdzdxbnz.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/genvkwxcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gspyqytrb.sHtML

[S51] C++：显式类型转换
来源：http://wap.zdbjq.cn/Article/details/gvvtltqgf.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gltgohnth.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gmfqkxzmj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gjrkvnlei.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/gokuvotuk.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/ggktxsuxm.sHtML

[S54] C++：异常处理
来源：http://www.blog.hesvh.cn/Article/details/gxzojsumc.sHtML


<!-- 参考信息 -->