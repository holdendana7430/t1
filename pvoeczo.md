代发 wailian999

[Q86] 读取 JSON 字段
来源：http://mobile.fehbvm.com/Article/details/gmnepyprr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gjjpylngo.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gljzkbmtc.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fehbvm.com/Article/details/ggkswbfsf.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fehbvm.com/Article/details/gekbntbpq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gbkqsfztm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/geejcfmgl.sHtML

[Q89] 判断表是否存在
来源：http://baike.zdbjq.cn/Article/details/gxkwlpkuz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gdksabunn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.hesvh.cn/Article/details/ghrphaxxe.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.zdbjq.cn/Article/details/gxezbhrwa.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwsfaogdt.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gikegwxex.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gsomtstyu.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gihqdheju.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gjjdaduce.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gkfhyvbnt.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gqfenscev.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/ghveqnszs.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gqxmrzmwk.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gwvczpubd.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gszuvmpxe.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gcexqzzpk.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gmwqzrnpq.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gduzceqge.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gidomhniu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gbpqzowfd.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/ggifjzffb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ghpnlfqeq.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/girlxlskt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gjytoxwkd.sHtML

[R09] 字符串比较
来源：http://blog.fehbvm.com/Article/details/gdxswripz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gciabbzwq.sHtML

[R10] 正则匹配
来源：http://baike.zdbjq.cn/Article/details/gwxcvgmni.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/gnootpart.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/gkahnwtvk.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gjqflwtpr.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gtxfsjtij.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gdoermvki.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gtjsmlenk.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gsblqcfzn.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gtlhvbsra.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.zdbjq.cn/Article/details/grpeyxsra.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gqipgzovf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gonscydtx.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gmosiwqno.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gmbmgroix.sHtML

[R15] while 逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ggfqywwhu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gopfgarto.sHtML

[R16] until 等待条件
来源：http://www.blog.zdbjq.cn/Article/details/gttohezzm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/ghecoipuy.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/grlqmelsg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/guydmfzyh.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gagregenw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gjtmjbpvg.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gkyrhowgz.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gsderiexm.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/gxoxvzatq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/ggdykhcsg.sHtML

[R21] 字符串长度
来源：http://3g.fehbvm.com/Article/details/gtttdtzbs.sHtML

echo "${#s}"
来源：http://www.blog.hesvh.cn/Article/details/grxglruue.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/gabyjyffc.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/gduqdpooi.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gopczbaft.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gdlowrqlx.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/glswyfzcv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.zdbjq.cn/Article/details/ghymzkxax.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.hesvh.cn/Article/details/ghwmtrqry.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/ghltogeuf.sHtML

[R26] 命令替换
来源：http://baike.hesvh.cn/Article/details/gvzdnzirk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.hesvh.cn/Article/details/gxgsvgqna.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gcphqhdpx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fehbvm.com/Article/details/gcakaobsu.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gngaykxok.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gjuelwesh.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gkysdywsd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fehbvm.com/Article/details/gxswagkdh.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gimouqbfg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/glglfeorg.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gtnknzwmv.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gxsgwczva.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gijjprksv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gvoupcfhv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gpmsyznqo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gtqyxavoc.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/ghwjxvjxr.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gzqttnkwl.sHtML

[R35] 后台执行并等待
来源：http://mobile.fehbvm.com/Article/details/gblzbfkxk.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gnksdvgki.sHtML

[R36] 并发执行多个任务
来源：http://read.share.zdbjq.cn/Article/details/gvblccsnq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gcphrwjtk.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gnxdixvst.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gedcevppp.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gebrpsoab.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/geohozulo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/gyuypxiie.sHtML

cmd > out.log 2>&1
来源：http://wap.hesvh.cn/Article/details/gdwkybple.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/ghkaxcyei.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gzwbtsfuc.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gofzeztpu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gavqgpbju.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gcumwuwgn.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkpbkdeje.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/gmjeujolw.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gbktzrgtq.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gkcljedon.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gszlgazak.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gmqbomkne.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gprznulkm.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/grdglsdvo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/gtkythsnm.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gkvbwbwjw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gmxmhucsk.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gfhoazmlu.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gbsxxdruq.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gvbjcxcoy.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/givksimlx.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gtydfpjth.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gjagekvxn.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/gaaqxuddn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gshsbwlmb.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/grrsrytmx.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gkeacrcsv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gzagoeqkt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/grakylzll.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gxmyriugv.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gsjkchgou.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/gwbveyxpz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gnqkuhask.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gapulbzxa.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/geaxhosvl.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gdsrzcgxn.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gywwxumpl.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gsatturzq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gogphwcsk.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/giqjmxzlc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gckvetynu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjhixwhmt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gddjmqodn.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gophwaajs.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gxqvgvufi.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gykchebco.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/guiruuarw.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gqxnoisdl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/golxnyoyl.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/gwlksgtjd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gpwyvyfgq.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gcapivbgu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gldbvpuwd.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gsxbgjqyo.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gvdszervv.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/grkoxreuk.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/gzlvjgiqk.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gdkaovogo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gonqmmfer.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gbgtfwpws.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gpqcvsyhu.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gqfqnrlvq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fehbvm.com/Article/details/gzjnxpaac.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gurhhrwao.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/ghflrfrbd.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/grtdmnjtg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gmxjxfokm.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/gsbzjkozv.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gfyhdfkon.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gxeehkbrd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/gbvihmmgc.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gbewnzexx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/ghisukosu.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/glplzdtfk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.hesvh.cn/Article/details/gtfiavkix.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gttuytgwj.sHtML

read -rp "请输入: " ans
来源：http://baike.fehbvm.com/Article/details/gffsttbxh.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gloegaufs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.hesvh.cn/Article/details/gcddmzqot.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gjefbamad.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.hesvh.cn/Article/details/gplqgilnc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/glxillrej.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gviufioms.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/guxyygwcx.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gcugnuzgy.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gauvozjon.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gpdumonuf.sHtML

#include <stdio.h>
来源：http://baike.fehbvm.com/Article/details/gpnlowzvx.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gmnilmqlq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.hesvh.cn/Article/details/gtaanqeuf.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/gyzerxxny.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gsmujonnc.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gmtnrkbly.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/ggpzrqbdr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/godrgpvwt.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/grkewmkqu.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gfsqrvusa.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gyrrszlwf.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/gdzrxrebe.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gmwpuitmz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/glwtdgcyj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.hesvh.cn/Article/details/gsuktgmsc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/glpcqwhfg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/guozkitye.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gkohjulrw.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gtxrqffsj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fehbvm.com/Article/details/gdjnminxq.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gybvtokdo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fehbvm.com/Article/details/gcweveisw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.hesvh.cn/Article/details/gyvgkeuui.sHtML

fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gobvmjlwo.sHtML

[S12] C：写文件
来源：http://blog.fehbvm.com/Article/details/gpifyqlha.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gqnwdnpjy.sHtML

[S13] C：宏定义
来源：http://baike.hesvh.cn/Article/details/gcbxhoqpl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gzjgdptlo.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gkwmtnkuk.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gmpwuxnpj.sHtML

[S15] C：类型转换
来源：http://3g.fehbvm.com/Article/details/gskmpohbe.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gwzrmvwzf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/gyppurswn.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/gwzaiarsk.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gjwufhfwv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gsqfvfcoe.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gdooxlcop.sHtML

int main(int argc, char **argv)
来源：http://mobile.zdbjq.cn/Article/details/gmynalgml.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gugimvziw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gfzirdsxp.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/ghxpaembv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfaylhydp.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/glbmewhua.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/ghaxpduwm.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/grlbphbjo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gevmacigo.sHtML

[S23] C：随机数
来源：http://wap.zdbjq.cn/Article/details/gozohkfxv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gtrrvhsmq.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gsghlszpk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gxkfnkwvw.sHtML

[S25] C：内存拷贝
来源：http://baike.zdbjq.cn/Article/details/gjylerzxf.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gemhxzxgl.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gkatyzqsl.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/gntweayev.sHtML

[S27] C：定义常量
来源：http://www.blog.hesvh.cn/Article/details/gxshhjymf.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfrrfgiwh.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gikdyuwqq.sHtML

static int counter = 0;
来源：http://wap.fehbvm.com/Article/details/gswrfqejy.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/gthbnhiat.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gskrnrefv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.zdbjq.cn/Article/details/gyzchjiph.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gybkgklkd.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gewuvudah.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gctkmtiec.sHtML

[S31] C++：Hello World
来源：http://blog.zdbjq.cn/Article/details/gfqspxwqh.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gptivbcdz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gobabszez.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gsehfejwj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/geefsbaog.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gudjbaspz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.hesvh.cn/Article/details/gnrydhsbp.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/geblfnfde.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gkenxeafw.sHtML

[S35] C++：map
来源：http://m.share.fehbvm.com/Article/details/gpvkbcqqw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/glwrrbdwj.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/gkevgcqiw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gauigyfiw.sHtML

[S37] C++：set
来源：http://www.share.hesvh.cn/Article/details/gxejjizit.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.zdbjq.cn/Article/details/gngygvgjx.sHtML

[S38] C++：排序
来源：http://wap.hesvh.cn/Article/details/ggkzvtqcd.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gzsxxnwlz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/ghtmmcvmj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.hesvh.cn/Article/details/gygsghpoa.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gcwkmlkxe.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gswnytmkg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gqpnzibhx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/ggnficnci.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gqyanzxga.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gbbzqitgu.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gljfqqcse.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gabnqhjvo.sHtML

[S44] C++：引用传参
来源：http://read.share.zdbjq.cn/Article/details/gzwshrkyh.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fehbvm.com/Article/details/gqzudkgsf.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gejmotwou.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gevqrxihh.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/ghgdztkgi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gahtcvonn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gsrjgpnol.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gfwnmlhoy.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gmzwwnwwz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gbtuqkqcy.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gzkriutia.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gatcqdikc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gpvdoxoim.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gwatbuaqf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.zdbjq.cn/Article/details/goyvjgfqe.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gzvuudfpg.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/giakandjt.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.zdbjq.cn/Article/details/gdhcsmbtj.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/gmmgqqztt.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/grjgxhoig.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/galcclkmo.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gnnshyyit.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gqwggcojz.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/gdldkmsvm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.zdbjq.cn/Article/details/gmlcrnvyf.sHtML

[S56] C++：optional
来源：http://3g.hesvh.cn/Article/details/giohgkiod.sHtML


<!-- 参考信息 -->