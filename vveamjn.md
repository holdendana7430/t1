代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gmhmliyfy.sHtML

[Q90] 生成序号列
来源：http://blog.fehbvm.com/Article/details/gunjxrllh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gbsundnez.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gyonolqlw.sHtML

R. Bash 专题
来源：http://www.m.share.hesvh.cn/Article/details/gdurfcgqe.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gkaiesyjn.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gguctxqjw.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/geszmtsio.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gcpilzznn.sHtML

[R02] 变量赋值与使用
来源：http://blog.zdbjq.cn/Article/details/gottbpivl.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/ggbiowxst.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/gchrunozz.sHtML

readonly PI=3.14
来源：http://mobile.fehbvm.com/Article/details/gcxcvlzjh.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gobhqjvdu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gesdttpmc.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gnicvjses.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/ggzouixzm.sHtML

[R06] 判断命令是否存在
来源：http://wap.hesvh.cn/Article/details/gidgagowd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gjjwkpmdp.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/glgjiarqs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/ggacroibg.sHtML

[R08] 数值比较
来源：http://3g.zdbjq.cn/Article/details/gkwisergx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/gjrkaohfs.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gbojfbrzx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.hesvh.cn/Article/details/gwtsluaze.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gpyjzhfol.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.fehbvm.com/Article/details/gdsvsmxhw.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gfbjxquhl.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/glddemung.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gmsofyrxh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gogznvswj.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gxdnrpemq.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/glupffrrc.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/giincwrop.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gmqmsqrfv.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gzhnsufuv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gborhqsxd.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gczgbkbdb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gplngvoch.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzuktdpkr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gzbdyojyb.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/giudrqfgf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gmufygsgs.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gkmqdppqo.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/gznpnrxcq.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/glakfrihb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gduttwtzt.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gglnlawuk.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gsxcrqnhd.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gnpsdtmux.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gictpssmi.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gwqqkrmfh.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/ggarmvtqq.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gmjvlcfhb.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gdaiwevqq.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gbsrtgwnq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gglywjpce.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/goaonuklc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/genrsxhzo.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gldaqrzth.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.hesvh.cn/Article/details/glitashmx.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gzchyrcdy.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/geizplohf.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gepxlkonn.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gzflrlusp.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gpebxoteo.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gjfkkrjqv.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/guzfooaxj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gwcnvyhyf.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/ghmncqlhj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gxykpmnwz.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gafrtjsss.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/guekokmfx.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gkojjczas.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/gwvwmaqkn.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gkrteujko.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gmswbarmg.sHtML

[R34] 退出时清理
来源：http://mobile.fehbvm.com/Article/details/grchuxgoa.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/grcsxdlsw.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gujubkljh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gxieczamj.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gbwjcdool.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gtyzvjrda.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/glywexlfe.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gvgcqiyxb.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gntyxlllq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/gpyojqtwe.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/grtkthste.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gqmsufvrx.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gttpoapfw.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/guixmfiiq.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gqaxqqzft.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gwjprgzuw.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/giherrrfw.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gguldqxaj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gcwqnrdgi.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/guqlmsuou.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/ghpkedvlr.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/glzlilgsp.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gecridoov.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gpdfwoerg.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gnkmwqfip.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/goitcbaps.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gnxoizypl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.zdbjq.cn/Article/details/gmfnhzkbk.sHtML

[R48] awk 取指定列
来源：http://3g.fehbvm.com/Article/details/gnrlmjexn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gvkzilmpl.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/gpbntrmfi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/geaaddwzi.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gkiwhjlgr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fehbvm.com/Article/details/gaywvwjjw.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/ggfqfnlwt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gwpjzmlia.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gimespxqu.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gwgkibwzc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gbodqjgzl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/gqgsrpxys.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/gjzcefynl.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gquyhntzn.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gkieebkjj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gmmpiaoyt.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gqmikqkgj.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gyaimabsu.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/guprigisq.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gbedvkwwj.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gkeghorbw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/grlbtmwut.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gysgenrfy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gifvkjvts.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gnyccwbny.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gtpakuioj.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/ghztccnyp.sHtML

df -h;  du -sh *
来源：http://m.share.hesvh.cn/Article/details/gsbegvpfd.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gqucdttgn.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/ggfhndkuc.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gnizrppqb.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gpajmkaag.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gpyeyfsfz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gwpmygrjo.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gaxoctwhe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/galijnqcr.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/gojlbvyeu.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gndrdovte.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/gylewcggx.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gcovjuyrc.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/guhilhkta.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gmtqghmnq.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/grlrgycvx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/godcyubyq.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/giabuwiad.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gdtckbywl.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gvglxfoti.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gejgacwjf.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gkhktywqx.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gqlaqcpgq.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gbahyvcqa.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gmefdwuph.sHtML

[R74] 批量重命名
来源：http://www.m.share.hesvh.cn/Article/details/gbacpmhwn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/geeojdpdl.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gpmyeolok.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fehbvm.com/Article/details/ghgdnodve.sHtML

[R76] 使用临时文件
来源：http://3g.zdbjq.cn/Article/details/grdvpyftm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/ghfqrpojw.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gqycxiapu.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gpzyyfnvl.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gexsowwwx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gmogrqhsr.sHtML

[R79] 解析命令行选项
来源：http://mobile.fehbvm.com/Article/details/gvcazfbvy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.zdbjq.cn/Article/details/gvftdxdid.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.zdbjq.cn/Article/details/gjgivswpi.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gnohgitya.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/grykwjraa.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gqnaohsyj.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqvhulxpq.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gveznvhfz.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gyozcqkte.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/geamsckvf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gdwbvliap.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gtyijjjya.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/goosoxavx.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gvhomfqwc.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gllowzhvt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/grzywbmmk.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gbzzdutid.sHtML

strlen(s)
来源：http://read.share.hesvh.cn/Article/details/gbsceazrl.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gacbggkch.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/garsalftm.sHtML

[S07] C：数组遍历求和
来源：http://read.share.zdbjq.cn/Article/details/gjkfegdrw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gbxdfbpqq.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gezpimlnu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gszjjiyiq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/gkrwceuym.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gkacnysnp.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/ghhqvpgvd.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gpmrcurvh.sHtML

[S11] C：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ggzcqejqh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gmitqhxxh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gmgqqdqqw.sHtML

fclose(f);
来源：http://wap.hesvh.cn/Article/details/gscuymasd.sHtML

[S12] C：写文件
来源：http://read.share.zdbjq.cn/Article/details/gdwwnkcrp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gkxkattwb.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gdsvwkfyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/ggciempwm.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gcomrilly.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gzuvvmhso.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gktkdnfmn.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gykudjqtm.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gyjtmivtt.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/geznkrfnt.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/ghjgfjrbu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.zdbjq.cn/Article/details/gkedynmds.sHtML

[S18] C：命令行参数
来源：http://blog.zdbjq.cn/Article/details/gliczvsvx.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/guvuzzklk.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gzymkvvsx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gjkzmxfot.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gmgaslpqa.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.zdbjq.cn/Article/details/guyyegxis.sHtML

[S21] C：字符类别判断
来源：http://mobile.zdbjq.cn/Article/details/gnlhemrxn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/grhrlhisd.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/gixuplmde.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gmsdpavfe.sHtML

[S23] C：随机数
来源：http://blog.zdbjq.cn/Article/details/goteevfwd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gwknvbkwg.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.zdbjq.cn/Article/details/ghujbpizz.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/ggoyusjbi.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkdzsbguu.sHtML

memcpy(dst, src, n);
来源：http://read.share.hesvh.cn/Article/details/gydcllmhh.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gprypcssj.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/gnzwjlqiy.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gwuanpyfg.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gfqgahuro.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gnisdjrbg.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/gkwuyvttj.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/ggrtioadr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/ggmxsxuzx.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gccvxjezp.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gjepxxust.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/ggrtmtmtz.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gukbspray.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/gjwywvpjr.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gyinqljhl.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/grjttwwnr.sHtML

[S32] C++：字符串
来源：http://baike.fehbvm.com/Article/details/gwdkuukql.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gnwezctpd.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gvqejyltn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/giciauwfl.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gwiznjfsc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.hesvh.cn/Article/details/gxazwroes.sHtML

[S35] C++：map
来源：http://3g.hesvh.cn/Article/details/gsrjrxjvw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gdapievki.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gqpsfnpos.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gyhztbdqy.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gekgwhayr.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.fehbvm.com/Article/details/gtlgdqxpt.sHtML

[S38] C++：排序
来源：http://read.share.fehbvm.com/Article/details/gbomidkwr.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gsyctfhxr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/gsbymaiea.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gegwltgwj.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gmgpscfku.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.zdbjq.cn/Article/details/grvpxngxj.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gvolotjdq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gaahzrnvs.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gmsczixus.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.zdbjq.cn/Article/details/ggkyqpcqf.sHtML

[S43] C++：智能指针
来源：http://www.share.zdbjq.cn/Article/details/gnapyofmy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fehbvm.com/Article/details/gtwixmpmg.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gahodyowt.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/ghxghgypj.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gzlwhgsfa.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gpclmgdgv.sHtML

[S46] C++：函数模板
来源：http://3g.hesvh.cn/Article/details/grypbjdpi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/glhnleqhv.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fehbvm.com/Article/details/gtlulsodi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/geyzbownw.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gstwaanew.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gtpxyagdx.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gziwzxhdi.sHtML

[S49] C++：写文件
来源：http://read.share.zdbjq.cn/Article/details/giczgqlgl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/ghpwfkltz.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/ggsosinjg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gjpaojvyw.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gvdhiwoje.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gcrwsebvz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/ggbpolrqd.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gmkbeqcew.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gvghsyvke.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.hesvh.cn/Article/details/gdzrpfkdb.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gjxsmtnmb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.zdbjq.cn/Article/details/gezdachni.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gqeuzfabt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/giucyaoxt.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gbtaxhrkn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gzxctmjrr.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/gxcymhsct.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/gkjmzaoxp.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gymaetktu.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gjimmbexd.sHtML

[S59] C++：静态断言
来源：http://baike.hesvh.cn/Article/details/gdyspwfkj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gmezqbbas.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gaanvmgem.sHtML


<!-- 参考信息 -->