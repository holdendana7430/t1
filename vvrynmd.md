代发 wailian999

set -euo pipefail
来源：http://www.blog.hesvh.cn/Article/details/gaqxaolbx.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gnryuczes.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gajhnfpnf.sHtML

[R03] 只读变量
来源：http://www.share.fehbvm.com/Article/details/gznkxwayd.sHtML

readonly PI=3.14
来源：http://m.share.zdbjq.cn/Article/details/gnacmxwva.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gxwstcfgx.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gdrybltwz.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gydsmwead.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/giuiljhep.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gzgltsnzq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gybwrxnck.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gkxcsbvuq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gvfautezt.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gqyhnlojl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gkdgxplns.sHtML

[R09] 字符串比较
来源：http://baike.zdbjq.cn/Article/details/gdulmexap.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gskiwalgm.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/giuwbkucg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gsurdmggg.sHtML

[R11] case 多分支
来源：http://www.share.hesvh.cn/Article/details/gfqeoqure.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gagzjgjci.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gfospknlf.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gzriugjwm.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gttnkloxj.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gymjgadop.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/gyndmakkd.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/gjpemhpff.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gcgwouzku.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/geypbgeft.sHtML

[R14] C 风格 for
来源：http://wap.zdbjq.cn/Article/details/geeodrofr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gjsipmnvx.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gdoducehe.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/gbfmwkhlz.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gpiqdywnb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gqreeirlq.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gbgftjsur.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gfnqnztqu.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/ggjmqqycn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/gmsjtyowy.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gsovwgsyx.sHtML

echo "${#arr[@]}"
来源：http://blog.fehbvm.com/Article/details/gnywngvuk.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/ggullpqqm.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.hesvh.cn/Article/details/gozvmupxv.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gepcratqh.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/grclwlkjy.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gikuqiuof.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gjrrpxofo.sHtML

[R23] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gekttsomp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gyfivqzjr.sHtML

[R24] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/ggyrxrkko.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.zdbjq.cn/Article/details/gwdceuwny.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gqojppqmv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gmnunetib.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gfuvhiwgv.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.hesvh.cn/Article/details/ggrcecwgo.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gzfaldcsm.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gsrihjvbu.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gaxxduuve.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/gnutnzjil.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gjmxhaeel.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/gogwqptmx.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gehaiopxy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gzyqcrsfg.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gxwxkxrrc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gleyyjsur.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/gmyfjdmrl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gfzpybhuu.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gtbsuctez.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gpvgztajd.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gvzgqronx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.hesvh.cn/Article/details/grfmayamo.sHtML

[R35] 后台执行并等待
来源：http://m.share.hesvh.cn/Article/details/gaclyvgnj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gyecqfywn.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gqyfvobny.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.hesvh.cn/Article/details/gawetlziu.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gjeqrjjhk.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gjyjtnmwl.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gzvmtyblh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/glbnxqwwx.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/gzdjmefmy.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gyauuxrxv.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gfncvcezu.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gkhamsjua.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gxjkjgjbm.sHtML

cmd >/dev/null 2>&1
来源：http://baike.zdbjq.cn/Article/details/gpiwkanhy.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/gvcxezhgx.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gufjvscev.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/glhqybykn.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/glawkjfyg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gjvzrmcsd.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gonkztvkw.sHtML

[R45] 批量删除
来源：http://www.m.share.zdbjq.cn/Article/details/gshznonxw.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/geuxrkoig.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gmaaoehqe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gpavikmxm.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gxmxcgmzc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gnrjtpfhy.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gkgwestcy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gtfpzcdli.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/goexvpbuz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gfvfamasa.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gxxsjkjyg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmaurxkbm.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gorlrqkpn.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gmclgxemb.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gtagpmuil.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gzdkperrc.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gatngydxy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gczmzsaki.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/gtnyrcevo.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gztanijgs.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gtatxubon.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/ghrdhfnct.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/goaowhnvy.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gyglwejnv.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/gywtnuxjd.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gblykjycu.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gywptuwzd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/glhbccrcf.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.zdbjq.cn/Article/details/gjohdzeop.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gdzwxygum.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gtsbbdyif.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gbfrdfzow.sHtML

[R61] 磁盘占用
来源：http://www.m.share.zdbjq.cn/Article/details/gebcaword.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/ggintekug.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gqyylhlja.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/grsclgazy.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/garkqilfe.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gfndqnjhl.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gmugwdexi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gcnkbkkai.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gtnfxddyn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/ggkhhwdei.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gfnyycxau.sHtML

crontab -e;  crontab -l
来源：http://www.share.fehbvm.com/Article/details/gtfnjiuud.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/glqguqapj.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gjklstfwy.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/ggvtjlkrg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/glrfusjga.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gowciszhd.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gqokwrrzd.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gmtrjeozw.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gtnhdacwo.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gmevhszjt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.hesvh.cn/Article/details/gsaqdxchp.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/ghnirktww.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzvyytmjb.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gnbncxgze.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gdwpwgpem.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gclccshrq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gfzsoxosv.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gejsordhi.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gkmycyuwl.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gfdammajg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gpqlnisit.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gmyiytxqv.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gqripqmyd.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/goajjyinf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gieeporzb.sHtML

[R79] 解析命令行选项
来源：http://mobile.hesvh.cn/Article/details/gyyimxmnj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.hesvh.cn/Article/details/guqebrtsa.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gkjvhjvbq.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/gwrpqztns.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gzribmyro.sHtML

S. C / C++ 专题
来源：http://www.share.hesvh.cn/Article/details/gcbgxnbrr.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfzkdxeef.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gyqgmincu.sHtML

#include <stdio.h>
来源：http://wap.fehbvm.com/Article/details/guzlqdmnz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/gdvsmvmxn.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.zdbjq.cn/Article/details/griwemxwf.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gfpbjtozt.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gzfbvpyqf.sHtML

int x; scanf("%d", &x);
来源：http://3g.hesvh.cn/Article/details/gyzbahqnb.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/ghharbjjk.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/gumzifuro.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gziwdthfb.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gzmautjfp.sHtML

[S06] C：字符串比较
来源：http://wap.fehbvm.com/Article/details/gbdueoxsp.sHtML

strcmp(a, b) == 0
来源：http://www.share.fehbvm.com/Article/details/gnupvjwvi.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/gpthmcuvo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gnoqtjswp.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/ghwcsjaks.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.hesvh.cn/Article/details/gypkhbrsk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gzhnosvgh.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gkzygpwgn.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gvkontqaj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/grjixieid.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gdrfnyfzp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gnkpfivaf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/gwsrnxfmb.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gpydfvwdz.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gsmshcrlf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/glrzhobem.sHtML

[S13] C：宏定义
来源：http://blog.hesvh.cn/Article/details/gpwxtwurm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gweruzplf.sHtML

[S14] C：枚举
来源：http://blog.zdbjq.cn/Article/details/gwbdhckhw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fehbvm.com/Article/details/gtoezrrmz.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gdiqduqyn.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gnclhksaa.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gnaoomwxj.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gfectimyp.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/ghdgkpvtb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/gggmogcqx.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gniygnbve.sHtML

int main(int argc, char **argv)
来源：http://wap.fehbvm.com/Article/details/gaamklhff.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gmblqbtmk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/gbiywtssh.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/grblxfdyf.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gpjwblmtj.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gcsrunwgr.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.hesvh.cn/Article/details/gfcuccvie.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gnlbxomnv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fehbvm.com/Article/details/gvmcnqplo.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gvskglrvm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fehbvm.com/Article/details/gljhufypb.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gbulfzifb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fehbvm.com/Article/details/gqfjjyfpf.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gmtvzgtnu.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.zdbjq.cn/Article/details/gufljbsjy.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gydlhundz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.fehbvm.com/Article/details/gozqrnbgk.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gubawvetg.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gjljveiey.sHtML

[S28] C：静态变量
来源：http://blog.fehbvm.com/Article/details/gxmytqjnw.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gpdxznkfu.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gozpeyewb.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.zdbjq.cn/Article/details/gsmjfeoum.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gtpqseqle.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gexdlorbk.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gznzalcbe.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gyibekhia.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gurhwuotj.sHtML

#include <iostream>
来源：http://read.share.zdbjq.cn/Article/details/giazsamkf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/ggageelhg.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gkyxydxih.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.zdbjq.cn/Article/details/gwvqfpuzb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/gkojpwirv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gternopqi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gjoiazncl.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.zdbjq.cn/Article/details/gqadoscrn.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gvkbnygsl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gdclazkht.sHtML

[S36] C++：unordered_map
来源：http://www.share.zdbjq.cn/Article/details/glcdhuuxu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gcumflxmi.sHtML

[S37] C++：set
来源：http://baike.hesvh.cn/Article/details/grpukmkzi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.zdbjq.cn/Article/details/gkuwambav.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gfwqqrvxq.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gjozqauzd.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gzhiegbje.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gifbjcqoj.sHtML

[S40] C++：查找元素
来源：http://blog.zdbjq.cn/Article/details/gfvlmpezi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ghmdbhkys.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fehbvm.com/Article/details/gsqizlqry.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gjrqsxqjb.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gkyeyzrlg.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.hesvh.cn/Article/details/gabsbxjob.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gdnbonpri.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gpvuqycwg.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gtfeigyhj.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gragmfpzq.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gsvopwtyf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.hesvh.cn/Article/details/gjvzkfhhc.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gmetiqdbi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gkluacrwi.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gsthnvotr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gnsluftnu.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gmwjlykgs.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gqkkgemfr.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/gqqknkrvg.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gwrqpahpx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gobufinkl.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gokicnmlx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.hesvh.cn/Article/details/gdzslqyui.sHtML

[S51] C++：显式类型转换
来源：http://read.share.hesvh.cn/Article/details/gfjsderbk.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gsuburvve.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/goxuiygvo.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gmfaenexe.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gzoxgymst.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.hesvh.cn/Article/details/gxbalhbuf.sHtML

[S54] C++：异常处理
来源：http://m.share.zdbjq.cn/Article/details/gbvfwyvlj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fehbvm.com/Article/details/gebkyzmhh.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/ghuhdcebx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fehbvm.com/Article/details/gyurlelyg.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gfnpjsnzu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gckzmgmsr.sHtML

[S57] C++：编译期常量
来源：http://www.blog.hesvh.cn/Article/details/gphyifpju.sHtML

constexpr int N = 10;
来源：http://blog.fehbvm.com/Article/details/gahaqbkbk.sHtML

[S58] C++：命名空间
来源：http://wap.hesvh.cn/Article/details/gcfwrcnto.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gcxyvswys.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/gfbwprjpa.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/gamjrviqe.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gvnckjaca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/guzkzacdp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gadsbcacu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ghuaexvql.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gpvmkoaam.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gnrzsldgn.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gtxmdogod.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gjotzhemw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.zdbjq.cn/Article/details/gplyokorm.sHtML


<!-- 参考信息 -->