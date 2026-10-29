代发 wailian999

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gwkarglrh.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gtsnspuzh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gqdnmolqg.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/grginusjx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gnfztkmue.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gjgjwmkyy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gdodtweve.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/ggnmblkjb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gxlqfupuc.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gwuskgxht.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gsenbhmfc.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gqfikgklg.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gmxafxmpf.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/ghsgilvoi.sHtML

stop)  echo "停止" ;;
来源：http://baike.zdbjq.cn/Article/details/gvmuhuytg.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gjbadpsnf.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gfyswbdpw.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/gyatpuoyc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gglsucdwv.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gwstmorue.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/geyudvtab.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/giaaakhpz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gcgyouwdv.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gjmptfujx.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/gwtpumzko.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/glnpwksbg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gazjphfch.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/gwlarrbpr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gnqrrvtgc.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gqfttimkl.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gmacvpgkt.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gtatubxzn.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gvrolvrbz.sHtML

[R20] 关联数组（字典）
来源：http://3g.hesvh.cn/Article/details/gkvnwfvdu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/grotezpuq.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gmtcuccuv.sHtML

echo "${#s}"
来源：http://m.share.hesvh.cn/Article/details/gkfddfsof.sHtML

[R22] 截取子串
来源：http://read.share.zdbjq.cn/Article/details/gcsxcexkh.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/geunvycjw.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gzuqqgzew.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gbevmjnkj.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gmcztlspt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gqcilmrmn.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gykegdwrg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/gyevxomvb.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gedrfacol.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gffitqcgr.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gnitszphr.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gcjpyjnln.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/giobmqwnc.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gglzmkjzk.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gsemsmkxj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gsmgzuqop.sHtML

[R30] 函数返回状态码
来源：http://www.blog.hesvh.cn/Article/details/gvqvlazna.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.hesvh.cn/Article/details/gkbkaomrf.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gargugkls.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gijaqbfec.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gxhrrzgai.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gzbnkfimh.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gjrthvanx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gymscopaq.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gawgivsur.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gfnjqoaqp.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gomgsnvgr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gdcdomtaf.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gglhmomti.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gujajksjk.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gszlupmdn.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gssufoaae.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/galrtmnon.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gqugxbclk.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gahdxtvmd.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gftjpfvgs.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/ghnhxfalu.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gnaaxkcqi.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gceaygofw.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gbybwqvtw.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gebtdhrds.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gknaiyedt.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gzfmwrwaw.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gseckibqn.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gnvqwqigt.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gxckefbyd.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gobmejtwt.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gebcrxzgn.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gcsixxumh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/grouujvhh.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gfontdouh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gzulzyxeo.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gicbojjos.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqzemftfv.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/ggyvafjyo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gfbmrtvjy.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gqelnxwey.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gxnzqnckc.sHtML

[R51] 排序去重取前几
来源：http://3g.hesvh.cn/Article/details/gexmrjczf.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gipsqfeye.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gdybviprp.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gllxsaohj.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.zdbjq.cn/Article/details/gcroklbgx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/glmuxhteu.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gdjlqrgsp.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gvymbvmlb.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gbftiepct.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gjanryave.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/guyoiubzo.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gjqtdwmyq.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gnzsqcels.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gpthllhwa.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gjifdeoni.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gtlkkiokz.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gautvfzpc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/grqlxcrln.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gbkgyrzdb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gmbbsalah.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gyblpzwpq.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gbjzzneyf.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gxfuhmwhz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gqlhkjymg.sHtML

[R63] 内存与进程
来源：http://m.share.zdbjq.cn/Article/details/ggzrmzjut.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gvvuqdzbl.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/glfxweajv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gjjqhaads.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gvdtlcmdn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gxhpsdvev.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gezjkogwf.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gnjdtybvz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/grznzckix.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gxxjfhipn.sHtML

[R68] 计算文件校验值
来源：http://www.blog.zdbjq.cn/Article/details/gscheqogq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/genhghoxg.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gmqgmkfqk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/galuiykbb.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gmhjqelir.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/ghyreajym.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/getucjtng.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gbhsqxdoz.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gsccvzqpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gpshteylt.sHtML

[R73] 分割大日志
来源：http://3g.hesvh.cn/Article/details/gnolamfwv.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gmbgrdrhb.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gwkvqlazg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gltcljixl.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/gifordrgu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/giqmfzxaf.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/geppkloms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gdekxzskg.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gwydrllqj.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/ghjzsxwqm.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gdmvqlblz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.hesvh.cn/Article/details/gttbhrvgz.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gsmyrduip.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fehbvm.com/Article/details/glppulhst.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/gxnkifwzf.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gsvmvfpbj.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gastkcqaq.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gmmjhbeod.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/ghhdbdsdz.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbbwmsikx.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gdxwbanad.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.hesvh.cn/Article/details/gtaaikddz.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.zdbjq.cn/Article/details/gelcgkgsc.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.zdbjq.cn/Article/details/glwyybrkb.sHtML

[S03] C：读入整数
来源：http://baike.fehbvm.com/Article/details/gznaaqrmw.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gnryxxxga.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gzwcnevjc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.hesvh.cn/Article/details/gakvbfymu.sHtML

[S05] C：字符串长度
来源：http://blog.fehbvm.com/Article/details/goaigaoea.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gqombphuz.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gfsmqqkyt.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/ggcwldvyn.sHtML

[S07] C：数组遍历求和
来源：http://www.share.hesvh.cn/Article/details/gjoazbssl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.zdbjq.cn/Article/details/gouxumudj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.blog.fehbvm.com/Article/details/gpwfvlzxu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.fehbvm.com/Article/details/gazqhrpmk.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.zdbjq.cn/Article/details/gerdggosl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gmssjayxf.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gvakaghrf.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/ghzavhceq.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/ghoozptkn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gxjxykcaf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.hesvh.cn/Article/details/gghgqmsjy.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gcraffkcz.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwojpjexq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gbxxehigo.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gvgqvxcmf.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.zdbjq.cn/Article/details/guavmiqel.sHtML

[S14] C：枚举
来源：http://blog.fehbvm.com/Article/details/gupbyxrfy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.zdbjq.cn/Article/details/gczyojpwv.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ginualjof.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gynaquzwr.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gfsqdjlyv.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gwukhyeup.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gxwgphkev.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/gprrmbdqt.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/grxdxhshu.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/gvjyzcrdn.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/ghsvrazpe.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fehbvm.com/Article/details/glykmrnym.sHtML

[S20] C：二分查找
来源：http://3g.fehbvm.com/Article/details/gxpkjqjez.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.zdbjq.cn/Article/details/grbkdqpwq.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/glykobyvp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.zdbjq.cn/Article/details/gupcygkuc.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/ggfojtkid.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.hesvh.cn/Article/details/ghktmnmts.sHtML

[S23] C：随机数
来源：http://www.share.zdbjq.cn/Article/details/gndkmmvyx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fehbvm.com/Article/details/gknenacox.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gnlkfvwko.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/grqwqkfzr.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gcmfehtoq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gisbkovpl.sHtML

[S26] C：内存清零
来源：http://www.share.hesvh.cn/Article/details/gtnunnrkp.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gjczistfm.sHtML

[S27] C：定义常量
来源：http://m.share.fehbvm.com/Article/details/gcxffdqlo.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/glydetqiy.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/gwhqlorpf.sHtML

static int counter = 0;
来源：http://m.share.fehbvm.com/Article/details/gnkwfskjn.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gussukvhp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fehbvm.com/Article/details/gshmbiicr.sHtML

[S30] C：头文件保护
来源：http://blog.hesvh.cn/Article/details/gqpthajxo.sHtML

#ifndef X_H
来源：http://blog.zdbjq.cn/Article/details/ggxeluigx.sHtML

#define X_H
来源：http://blog.fehbvm.com/Article/details/gzxgtepgu.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gfwkmospo.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gcbrdfric.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gjntcymta.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.hesvh.cn/Article/details/gmmpaeptz.sHtML

[S32] C++：字符串
来源：http://mobile.hesvh.cn/Article/details/gmuyqbapn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/ghgskoprk.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/gdnrzvctn.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gljymthji.sHtML

[S34] C++：遍历 vector
来源：http://3g.hesvh.cn/Article/details/gteyzspib.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/gspgptplb.sHtML

[S35] C++：map
来源：http://www.share.zdbjq.cn/Article/details/gpcxsqjbf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gppzmpprs.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/glfszotvr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxsnzczpm.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gxlnxyfip.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gqbfrequq.sHtML

[S38] C++：排序
来源：http://read.share.hesvh.cn/Article/details/giwmlplbr.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/glusaotsq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gxscotgqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fehbvm.com/Article/details/gwepvgbhq.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/gkummqwuk.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gaqrxlijo.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/ginphrgod.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.zdbjq.cn/Article/details/gdtpxbynz.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/gkjslmees.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.hesvh.cn/Article/details/gsygpvntg.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gcdshviue.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.hesvh.cn/Article/details/gxmjofyhu.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gsvahfqns.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gnzeokqfl.sHtML

[S45] C++：lambda
来源：http://baike.hesvh.cn/Article/details/gttxbdtlr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjrflcekd.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/gcebytusu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gyxepylut.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gfmpzbsjf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gtzlqkara.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/ghsxaivyf.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.zdbjq.cn/Article/details/gfocwwuvo.sHtML

while (std::getline(in, line)) { }
来源：http://wap.hesvh.cn/Article/details/gufulrquz.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gqneblxuy.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gkwbxrvbd.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gmyqqrlzk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gneqiwuys.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gxvglsruv.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gmiivoujc.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/glasuzggv.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.hesvh.cn/Article/details/gsxpyuimy.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gyiodheyz.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gnuisvjyb.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gcwbdlwzw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.hesvh.cn/Article/details/ggytgbqaa.sHtML

[S55] C++：结构化绑定
来源：http://3g.zdbjq.cn/Article/details/gtgdwrcxx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fehbvm.com/Article/details/gmkadmkqb.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gugyisdoh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/grrlrkeov.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gtjdmhfov.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gftimsvcu.sHtML

[S58] C++：命名空间
来源：http://baike.zdbjq.cn/Article/details/gdxupahmf.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gtwdmevzk.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/gjcadaefk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/ggowjhpmq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gmzioikle.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gxawcbpxk.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gfeibwrsf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.hesvh.cn/Article/details/gnxvulirj.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gfpxseuxe.sHtML

[T01] Kotlin：Hello World
来源：http://blog.fehbvm.com/Article/details/gogfhrsoe.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwuvjlmrf.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gdoabzdxt.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gqmtvbyfa.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gocpcbyhk.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gkkwwfxyj.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gxjixrriv.sHtML

val n: String? = null;  n?.length
来源：http://read.share.hesvh.cn/Article/details/gpbegsxxr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/grredinbw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gjkxpwdrs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.zdbjq.cn/Article/details/gfhebyooj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.zdbjq.cn/Article/details/grqjntdjv.sHtML


<!-- 参考信息 -->