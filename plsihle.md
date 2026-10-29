代发 wailian999

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gtszuyruq.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gmtdvpvee.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/githcbfbr.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gjhwrixqs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.zdbjq.cn/Article/details/gzlrksndz.sHtML

[R08] 数值比较
来源：http://read.share.fehbvm.com/Article/details/ghezvbkuc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gkunsulma.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gknwtbulx.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gumhkpqst.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/gybrqjxtq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gvlbxfdgg.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gkqpcagpo.sHtML

case "$1" in
来源：http://www.blog.zdbjq.cn/Article/details/gsmotqzor.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gdvgmjvln.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/gyktufafl.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/glhbbtpew.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/ggbnhgymf.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gqwowpnix.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gykwsphry.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gxouzfpmv.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/grjvbgwvn.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gbcpawnfz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gerjcwgrx.sHtML

[R15] while 逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gqtvutciy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gswglwfbu.sHtML

[R16] until 等待条件
来源：http://www.share.fehbvm.com/Article/details/grfnjirwo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gwyrxucos.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gtsbkpbrb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/guylahkas.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gubedpdna.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gilyyajsq.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gbfyauibi.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gcwsunpoi.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gqtownuhs.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/grjozlcyl.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gadvlydip.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gnxpqzalz.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gfxbavaim.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gdvktjwqn.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gideiifbf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/genringfi.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/goqpiddlc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.zdbjq.cn/Article/details/giyfqpifo.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.fehbvm.com/Article/details/gpexdbdyq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gixqjqfoy.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/gvzwpmbcl.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gcojtpxnt.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/giecjnmev.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fehbvm.com/Article/details/gslvlbhwc.sHtML

[R28] 浮点运算
来源：http://www.m.share.fehbvm.com/Article/details/gopfkvtcs.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gheobrebu.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gtyovtwxn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gjycjbgif.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gasqlgiur.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gmblpbqkr.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gkzdpmqaw.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gmnrvhmcq.sHtML

[R32] 参数个数校验
来源：http://www.blog.zdbjq.cn/Article/details/guapkevxz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gcewpolak.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gmreovzfe.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/gnpjdzlrd.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gzcqxirfh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.fehbvm.com/Article/details/gckzwkibf.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gpevglunv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gpmopvods.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/ggkwwexpv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gtqveretm.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gtogxlrku.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/grfhlzlta.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/gbcbfvdeo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gruamioft.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gvpspdkpm.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gopspsrcv.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gevuyqaxt.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/ggbxzqbgj.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gnbdrppik.sHtML

cmd >/dev/null 2>&1
来源：http://baike.hesvh.cn/Article/details/gcydwuygl.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gydlndtwd.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/ghjbtrtts.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gaykaoegp.sHtML

find . -name "*.log" -type f
来源：http://mobile.hesvh.cn/Article/details/gwjakxilm.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/guzfihxzo.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gakbabtpv.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gichlfrhb.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gtykjpatv.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gbqdryfxd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/guwbblbyc.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gzdjwhqgv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/givqinxyz.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gqraoatbr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gtlwtjtwt.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/gzsvdztsl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gtcoyfikv.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/gfyzczwpw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gphdvynck.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/glveruteo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gljwixjrr.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gdjqgdtyf.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gecwgeabx.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gjfgzvydx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/genqcfjug.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/glxzhepne.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gpzrzodyx.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gunzijneh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gezxxlcse.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/geeueqbdy.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gqzigwywz.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gfaddbfci.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gbrsiiukx.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gqgsoawmv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/guaogbddm.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gfmriaacz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/geppqkkjd.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/grboqbwzm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gmllyjppa.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/grihdsojn.sHtML

df -h;  du -sh *
来源：http://read.share.fehbvm.com/Article/details/guozrhvvi.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gmfapfeqo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gmddhpgor.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/guluwrgad.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gtgvakopv.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/ggxnouhiz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gkqwwrhep.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gfweblebj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/ggpekimhu.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gywhqrbks.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/goqmnexld.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gyedxixzr.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gbvbyvgtm.sHtML

[R68] 计算文件校验值
来源：http://read.share.zdbjq.cn/Article/details/gvxpgnbrc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gjuhurfij.sHtML

[R69] 生成随机密码
来源：http://www.blog.hesvh.cn/Article/details/gvjttpiwc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gcizljufg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/galrrlrtg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.hesvh.cn/Article/details/gkgxxczdg.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/govlocsvm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gbtygtvbl.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gwrhqzkhc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/geuibnhjh.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gspqvmgwj.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.hesvh.cn/Article/details/gcvihajnp.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gsxabdtff.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gtebcogdo.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gausyqoxn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.zdbjq.cn/Article/details/gstjiefmj.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gropbtiet.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gzcxblsge.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/goiwapuum.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/gsanebozs.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gkcoozssb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.hesvh.cn/Article/details/gllygmwjl.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gvcbvzosa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gjswnoyhv.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.zdbjq.cn/Article/details/gnmzdcbiz.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gxvxynhms.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gkczmwgvi.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gojpnwjbp.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gvzirlclt.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/giqrvwpfg.sHtML

#include <stdio.h>
来源：http://www.m.share.hesvh.cn/Article/details/gmwkeorjg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/glspdfice.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gcvoftgod.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gtxfvpdes.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gwjkkboqt.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gacbqtecl.sHtML

[S04] C：字符串复制
来源：http://www.share.fehbvm.com/Article/details/gprtrxbnd.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gavbofrdz.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gxdpvyxjw.sHtML

strlen(s)
来源：http://www.share.hesvh.cn/Article/details/ggpaarlfj.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/giiyvpwif.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/grxeapprd.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gcmcvvsyv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fehbvm.com/Article/details/ggxlcmlpq.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/geewrpsmj.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/ggwcfmyzq.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.zdbjq.cn/Article/details/gpijhuxni.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fehbvm.com/Article/details/guubzyymu.sHtML

[S10] C：指针与解引用
来源：http://m.share.zdbjq.cn/Article/details/gneolkbmu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gxcgxkkcl.sHtML

[S11] C：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gezzsyxnw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.hesvh.cn/Article/details/gtofvdzaz.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gdegqraim.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/glknkbsmj.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/gfircmzar.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/gukemcqzx.sHtML

[S13] C：宏定义
来源：http://mobile.zdbjq.cn/Article/details/gxfdgrftd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gakmuifva.sHtML

[S14] C：枚举
来源：http://baike.fehbvm.com/Article/details/ggakmwylu.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gjbniiudd.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gsvotnwpe.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gscglpgfk.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gxqbolqre.sHtML

x |= (1 << 3);
来源：http://baike.zdbjq.cn/Article/details/gwayorfsi.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gtbewewvf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.hesvh.cn/Article/details/gljosvbmn.sHtML

[S18] C：命令行参数
来源：http://www.blog.hesvh.cn/Article/details/gllaamvec.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/garyhbxna.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gljlujgqg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gvhzjbfkz.sHtML

[S20] C：二分查找
来源：http://baike.zdbjq.cn/Article/details/gkwjfvsmt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gnhetuzia.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gensmoleh.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.zdbjq.cn/Article/details/gltrdpzey.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gcwmuwewq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fehbvm.com/Article/details/goacschfp.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gjbizfcqi.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.hesvh.cn/Article/details/gvptlowbj.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/glcnwlbpa.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gdvdrpqwu.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/ghqjrycqa.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gxzpzcruf.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gjgagyrml.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gpsjrjyle.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/glphfmbpa.sHtML

const double PI = 3.14159;
来源：http://read.share.fehbvm.com/Article/details/gbnoypsaa.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gfejvygmx.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gvfihpsto.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gcapnkhqt.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gywpgrdkl.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gnidudlfg.sHtML

#ifndef X_H
来源：http://wap.hesvh.cn/Article/details/grwggxhiu.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/ghaoxiogt.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gzaqqsnbo.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gktjwxfbm.sHtML

#include <iostream>
来源：http://wap.zdbjq.cn/Article/details/guiuohzjz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.hesvh.cn/Article/details/gvavurotu.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gtculrtjw.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gnroyabja.sHtML

[S33] C++：vector 增删
来源：http://m.share.zdbjq.cn/Article/details/gyaloohtl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fehbvm.com/Article/details/goiuwgaei.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gsuwqzxkx.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/ggbfhnkdy.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gopwgwgyb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/gwpetwdvn.sHtML

[S36] C++：unordered_map
来源：http://read.share.fehbvm.com/Article/details/gynsyzxiz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gyqslvpip.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/ghvsxyxgi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.hesvh.cn/Article/details/gknhfpjuc.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gygmvkyqm.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.hesvh.cn/Article/details/glztjwapf.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtvenliev.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.zdbjq.cn/Article/details/ggtjmwpge.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/grixtcjry.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.hesvh.cn/Article/details/gwirqhzau.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gufcqvnvm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.zdbjq.cn/Article/details/guojyusqb.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gktxgtgzi.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gvznzgizv.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gvchgtoxx.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gzqabqmjc.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/gpnxwokjs.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gslrtsaep.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/glyzunhtl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gjodehzib.sHtML

[S46] C++：函数模板
来源：http://blog.hesvh.cn/Article/details/gnhkrctyp.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fehbvm.com/Article/details/gpixkldom.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcfsucmkj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.zdbjq.cn/Article/details/gwiaqjsog.sHtML

[S48] C++：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/grrvdqqvf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gsgxzydxf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/ggmifrbup.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/gskpdpuhv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.zdbjq.cn/Article/details/gtcbecynu.sHtML

[S50] C++：格式化数字
来源：http://wap.zdbjq.cn/Article/details/gjrrofneb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gsbpwrsut.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/ghcjmrwvx.sHtML

static_cast<double>(a) / b
来源：http://blog.hesvh.cn/Article/details/gzynfpakb.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gvtpmwzgs.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gbsosgaad.sHtML

[S53] C++：移动语义
来源：http://wap.hesvh.cn/Article/details/gcxttdnnl.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.zdbjq.cn/Article/details/gutbowujm.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gdmljccba.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/gtxotjysn.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gotrhzmub.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gkresmelz.sHtML

[S56] C++：optional
来源：http://www.blog.hesvh.cn/Article/details/gcawiucho.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/gihgloeoz.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gaqbivewg.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/ginsbcvte.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/guylpbhuh.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fehbvm.com/Article/details/gzfmimssu.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gdcnaomci.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gpulxcutk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/glptnbscr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gerncbklc.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gofcnvanc.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gqwamfhyc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/glcuyjmbk.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gsjyfvpra.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/grbvewjgo.sHtML

[T02] Kotlin：变量
来源：http://www.share.zdbjq.cn/Article/details/gwtkuvxxv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gfcbbazji.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.hesvh.cn/Article/details/gibghuaiz.sHtML

"值: $b"
来源：http://m.share.zdbjq.cn/Article/details/gjtlnrvfj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/grvqipuhf.sHtML

val n: String? = null;  n?.length
来源：http://blog.hesvh.cn/Article/details/gdgkxdsdd.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gjjlfgjwg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fehbvm.com/Article/details/gsxyqamns.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gdbbvwhwr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.hesvh.cn/Article/details/glyebabiz.sHtML


<!-- 参考信息 -->