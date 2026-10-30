代发 wailian999

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/ghixyhzlf.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/gdpqnegnk.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gwrncegqp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gjsfznrdr.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/ghqtkjtta.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/guztsijti.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.hesvh.cn/Article/details/gpxclpvmo.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/giypcylce.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.fehbvm.com/Article/details/gnrnybuif.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gpyjplisu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.hesvh.cn/Article/details/gmegwmwyh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbyiqcoor.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gyfwgiail.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnyzuoesg.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gdxfvavfn.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/glqhfxeli.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/ghirwjcwx.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gityqfmqr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gpsdnsokl.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gbdjdbxjq.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gnrhjivfr.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/gitiixxrv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gsftrpsja.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/ghpjbjbre.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gxgxqxjqj.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gguhvvwgj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gwkimukbt.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gmayuhlpr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gibmsvbiq.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gqbqmturh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gtvxbixyf.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gzavodoxf.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/gcbofiqzt.sHtML

[R10] 正则匹配
来源：http://m.share.fehbvm.com/Article/details/guijedhnr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gtvbteymw.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gykmoljwm.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gprvxwrcf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gmebwohqb.sHtML

stop)  echo "停止" ;;
来源：http://wap.fehbvm.com/Article/details/gfyrbfpnb.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gukkudslv.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gxpaswwqh.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gxzmuhhxl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fehbvm.com/Article/details/gpvyxuhre.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/grzhlfkia.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/geymbqniy.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gqlicfuuv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gwazanhxt.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnofjbpiq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gpotvmdoy.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gnzltnhja.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gtgdluglc.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gccakrrfb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gfnjcmzer.sHtML

[R18] 遍历数组
来源：http://3g.hesvh.cn/Article/details/gqmfsqkrc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.fehbvm.com/Article/details/gmwtdpasq.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gvaohucjy.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gjpyghvpf.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gmftuhtvl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gjdnxskjc.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/geqyukmsy.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gandzxnqr.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/ghghahmfe.sHtML

echo "${s:0:5}"
来源：http://mobile.zdbjq.cn/Article/details/gntrfrnzb.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gxrpwghnr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gcuiwwiio.sHtML

[R24] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gcycrubak.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gngjklxqu.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gacscmguz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.zdbjq.cn/Article/details/giyclcrfd.sHtML

[R26] 命令替换
来源：http://mobile.fehbvm.com/Article/details/gdiqoxdzt.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.hesvh.cn/Article/details/gvnpczhur.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gwfwayuqi.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gskkbycto.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gphpphvkf.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/glrxyyuvf.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gkgujeniv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gzploxuep.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/gynpijphi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gfomzmnbb.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/golkxhigl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gqtoxqkom.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gthddfbik.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gmmzzunmq.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fehbvm.com/Article/details/gnqecvvki.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gzxwpyrsb.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/ghyatpodu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/gpqahzbmy.sHtML

[R35] 后台执行并等待
来源：http://read.share.fehbvm.com/Article/details/gtnpemyap.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gcuapaqek.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gclrbarek.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gwcbaoqss.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gsiahguvu.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/ghsmdutcc.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gdvfyarba.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gqnczftwy.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/ggctofvgn.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/glqmjsusg.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gqqzmovdm.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gpoothhlg.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/giefxwmnr.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gflwrytsf.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gtrkcezla.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gsijhibad.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gyovczlba.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gimhjvtll.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gosqenwaa.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/guwqxfhzj.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gumkcmusy.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gwxyxhzdy.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gmtmehzev.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gwdyznevi.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gbfxvntdf.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gsozhlxly.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gucldffll.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gkydkvsub.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gixpkvaut.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gtcryrdlp.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/grbrdbgkr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/glxhouspp.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/geqtzewlj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gmhamspqp.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/geugiqrgw.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gmnaexvrx.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gmdmjmnyd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.hesvh.cn/Article/details/glxxnihkg.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gcfzlovbr.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gouvnjfhp.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gehryhkzi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gsinpxebb.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gkaxjipky.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/gfbsmlpoa.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gzabeansi.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gmnewnqon.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gaoztlfpr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gvnmwzgwe.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gldzkftas.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gkogyxvgb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gidjodoar.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gjqasavcn.sHtML

[R61] 磁盘占用
来源：http://www.blog.hesvh.cn/Article/details/ghfszpjoi.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gecvgmjfs.sHtML

[R62] 找最占空间的文件
来源：http://m.share.hesvh.cn/Article/details/gzuivzyet.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/glcsfzbqx.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/gwwtcqegt.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gpbotohiw.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gbrgqjycx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gbcrnqurk.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/goxjoczkb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/guqchsyom.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/ggqnliogr.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gclibzdyk.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gxxrfzfuo.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gvlriakwa.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/ghjvaicmt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gthankrnu.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gumoivtwh.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gmhssfiad.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gpeqkclgl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gfygeyaaf.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gusjgzfct.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gnheakmkp.sHtML

[R72] 等待端口就绪
来源：http://www.blog.zdbjq.cn/Article/details/gvsifgeez.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gtvanmhme.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/gjjeojcvm.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gyauoaobp.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gaonbkils.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/gjkiutqvs.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gfmhkhdih.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gfduedwmc.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gzzkayhbv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gvztbvxru.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gjjbcwosk.sHtML

read -rp "请输入: " ans
来源：http://read.share.fehbvm.com/Article/details/giwdlmmrz.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gyqaozseh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fehbvm.com/Article/details/gychwgjrm.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gdrcxxubp.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/gwhxpuzkl.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gewnuuoap.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gdxvaqhrw.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gegqfvumn.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gciydlgac.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gbejtgclm.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gkhfckxel.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gggadtfzw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.zdbjq.cn/Article/details/gceuyemqr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fehbvm.com/Article/details/gcgahbwht.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gqdmfwwdl.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gnvqlxmrx.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gjmxjrdte.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gxwjahfda.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gdqivaqhi.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gdiidftqy.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gayfgpmjg.sHtML

[S06] C：字符串比较
来源：http://wap.hesvh.cn/Article/details/gfhsfwgqk.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gzbdnjxnb.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gtdgzlwdu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gkgcfpvrn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gliedjdzh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gqbxpmdoi.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/glmnleaof.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gywnktyst.sHtML

[S10] C：指针与解引用
来源：http://blog.zdbjq.cn/Article/details/gizsoyvrp.sHtML

int *p = &a;  *p = 5;
来源：http://3g.fehbvm.com/Article/details/geeyhwlls.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/ghyjasybr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gwbnywtmq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gjiycskov.sHtML

fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gfghscnag.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gkmpskxty.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gjbcytzgj.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gufxyrtig.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gatkjggqd.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gwqatskvy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gadsnvakw.sHtML

[S15] C：类型转换
来源：http://3g.zdbjq.cn/Article/details/gtaafrvoi.sHtML

(double) a / b
来源：http://m.share.zdbjq.cn/Article/details/grviflzpm.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fehbvm.com/Article/details/gnvbdwlth.sHtML

x |= (1 << 3);
来源：http://3g.zdbjq.cn/Article/details/gvrvkuaxj.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gdpxkngjt.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/gimqrttsz.sHtML

[S18] C：命令行参数
来源：http://m.share.zdbjq.cn/Article/details/gdkunwnvo.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gkyhjqsew.sHtML

[S19] C：快速排序
来源：http://baike.zdbjq.cn/Article/details/gxfxebxxm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/ghxnojhsg.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gbmtqijwb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gaczfeauw.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gvlxxmbca.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fehbvm.com/Article/details/govlzrtss.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gcdokocdy.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/gggspeuph.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/gvwvsebmp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/geeahnegd.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/ghcjhdjvn.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gjtzymjsp.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/gwvrtnebx.sHtML

memcpy(dst, src, n);
来源：http://wap.hesvh.cn/Article/details/gdwzpvcqa.sHtML

[S26] C：内存清零
来源：http://www.share.zdbjq.cn/Article/details/gftagshkx.sHtML

memset(a, 0, sizeof a);
来源：http://baike.zdbjq.cn/Article/details/gfiezzvqd.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gchewmadt.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gsexqncfv.sHtML

[S28] C：静态变量
来源：http://wap.zdbjq.cn/Article/details/ggjwijyjr.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gdeowqulm.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gclkjrnbg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gwwynjaac.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gwrugmzja.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/glaidywkl.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/glihqakyl.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gpmaiwlyq.sHtML

[S31] C++：Hello World
来源：http://www.share.fehbvm.com/Article/details/gjbkriiin.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/grgcktfrj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gxkqvgzsq.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/gpwscugwy.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gsgskgimc.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gcuxmksqh.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gufugxbdl.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/geuwquacr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gqmsxooxa.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gvxladakq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/glujwrgku.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gzxtotqdt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/guusqoruw.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gjkmlxzza.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gzzbsqpim.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gvkpggahv.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gzzhypzpo.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.fehbvm.com/Article/details/gollpdyep.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gckegihhj.sHtML

[S40] C++：查找元素
来源：http://m.share.zdbjq.cn/Article/details/gjqtggocb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/ghmwgrqlp.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fehbvm.com/Article/details/ghdulvtra.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/glmwmiasm.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/ghcpnfhjo.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.hesvh.cn/Article/details/gjwyqahna.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gdhdwjnqd.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.hesvh.cn/Article/details/gksxosmki.sHtML

[S44] C++：引用传参
来源：http://wap.zdbjq.cn/Article/details/gyyvxkvzy.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gyvablxsh.sHtML

[S45] C++：lambda
来源：http://read.share.fehbvm.com/Article/details/gzofulldo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.hesvh.cn/Article/details/gucznoddr.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gcmjjwkuw.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gjpfmltrg.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gaaysolxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gkejqxsyp.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gdurxndvm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gdelzsyey.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.zdbjq.cn/Article/details/gptmtyrlr.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gmziieupp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gcwcyonjt.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gahihpawk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gwxzqmskc.sHtML

[S51] C++：显式类型转换
来源：http://baike.hesvh.cn/Article/details/ggkovnjnj.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gmxnxbqzt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.hesvh.cn/Article/details/gewxltdpz.sHtML

int size() const noexcept { return n_; }
来源：http://3g.zdbjq.cn/Article/details/gdiydgvie.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/ggfyyglhw.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gmxikmhjn.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gbdqbqwdn.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.hesvh.cn/Article/details/gqluhjjnr.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gvgvlbccw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.zdbjq.cn/Article/details/gnhadhetg.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gtibvtzcs.sHtML


<!-- 参考信息 -->