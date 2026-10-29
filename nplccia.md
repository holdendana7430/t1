代发 wailian999

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/ghgcdsrdd.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/giqwptfga.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/guafairad.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gecqtbpjc.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gtrlswmwb.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gwuknyhwq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.hesvh.cn/Article/details/ggliyjzwd.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gmclvpves.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gydtnaknv.sHtML

[R14] C 风格 for
来源：http://blog.hesvh.cn/Article/details/gvuauneeh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/gehlewysh.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gghwzawab.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gnenvlcxm.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gwcycfazs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gmcgwwmaf.sHtML

[R17] 数组定义与取值
来源：http://mobile.zdbjq.cn/Article/details/gnaljsnuf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/gdlmrzslc.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gqcmrphwx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.fehbvm.com/Article/details/gkxocldic.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/giymaqycr.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gkjnflbpz.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gowfstbwz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gqxpncbae.sHtML

[R21] 字符串长度
来源：http://wap.zdbjq.cn/Article/details/gggbrsuch.sHtML

echo "${#s}"
来源：http://m.share.zdbjq.cn/Article/details/gzkwdizep.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gngrrnsgj.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gzykgwkdd.sHtML

[R23] 字符串替换
来源：http://wap.hesvh.cn/Article/details/gweydmefz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gmebbnmvc.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gbxjfnluw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gwbelvbrj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/ggkyqdqsr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/ggduccvmi.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/ggnbxrfwr.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gafsmhaue.sHtML

[R27] 算术展开
来源：http://www.blog.fehbvm.com/Article/details/gwxuusiyb.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gluegfnye.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gejmvealt.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gnrzscfva.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gzldpvehs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gshywjjxs.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fehbvm.com/Article/details/gwwjbqshj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gcevsvpyw.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gxkcjwiru.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gjzrhqrjf.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/gctsnxacz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gxovwkzdd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/ggxtpmjwt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/glvktjuvd.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gwggrwigi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gwarjbbfv.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gjlpstmrq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gemahltxd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gwnwmkgla.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gdxjbjxkk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gkwkgzwcl.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gjhjxqqyi.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gtizpxtln.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gblnsrata.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gkipfxjrr.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gzvswahme.sHtML

[R40] 追加写日志
来源：http://blog.zdbjq.cn/Article/details/ggiiwigxm.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gkjmjlklp.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gbvaldxol.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/gvwdywsxp.sHtML

[R42] 输入重定向
来源：http://www.share.hesvh.cn/Article/details/gxhjxmhvb.sHtML

wc -l < a.txt
来源：http://mobile.fehbvm.com/Article/details/gdrgqsqtf.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/ghwmwvpll.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gyjqvrack.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gtgnzxtxk.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gasxigqyn.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/ghodtilhv.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/ghmwamwto.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/gvbfoebss.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/glqmchyzj.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gqjxboaap.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/ggpukgemo.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ggexmuair.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gmpzzfncg.sHtML

[R49] awk 带条件
来源：http://m.share.hesvh.cn/Article/details/gprbsebuw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gwtbwiqhj.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/gyosuchmj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gvwrgizvv.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gjzykmwmt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gdbjgqfxg.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gfrorzdbd.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gxqkolris.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gsyvtguqs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gvqcfmvzb.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gumedbfhp.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gfzezsgpi.sHtML

[R55] 压缩与解压
来源：http://3g.fehbvm.com/Article/details/gzyuwcmyw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/glkzwoufz.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gjhbxotts.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gvwlcenlg.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/giannflob.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/giqxcfnuk.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gcuwlpxiz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.fehbvm.com/Article/details/gtppavstb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/geffynwhd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gepylcpzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gxdcdnnog.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/githjfdlp.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gkrpzazde.sHtML

df -h;  du -sh *
来源：http://baike.zdbjq.cn/Article/details/gwhnjtpgf.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gujoxkscn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gxhupmueg.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gcpvobpgk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gwdnmcrdp.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/getozyftm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gjrbhdofv.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gkxcguhgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gampjgsmr.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gncigxxzm.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gskhewany.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gagqfcztz.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gblqedpof.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/gwsfergcy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gujbduyjo.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gfwmxqgag.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gbrkcssiv.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/glbgoqvxd.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gzuuzfcwc.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gaduskivq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gnnzsobey.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/ggkcmoyck.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gqpmienhv.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gucumetry.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gxarcsecl.sHtML

[R74] 批量重命名
来源：http://mobile.zdbjq.cn/Article/details/gibawsmrk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/ghexwowgc.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gawutdlvz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/gntclezwh.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/gxsinuiao.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gviyjnrox.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/grvladptm.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gpcjdawpx.sHtML

[R78] 交互式菜单
来源：http://www.blog.hesvh.cn/Article/details/gxwpzgeeq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gmbpsovcc.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gegnecqpc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gpswqhaov.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gqbizgeqf.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gnisektbs.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glkmzfafm.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gutiksujv.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gurxtozja.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gbyevfqiq.sHtML

#include <stdio.h>
来源：http://www.share.fehbvm.com/Article/details/gdmhmrxjr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.hesvh.cn/Article/details/gslbzbfnb.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gobnetktd.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/ghpvziqby.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gaehucliq.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gjdfgmpzi.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gaxukgfsc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/gumkjkeyw.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gfksxpbcx.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/ggqgtzoth.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gtqlvjgvn.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/gemnpkgay.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/goiwjwpbs.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/ggtrulmgi.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.hesvh.cn/Article/details/gcpzvcwav.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gnlbcqpxc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/goyfmesmx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.hesvh.cn/Article/details/gmqenkwly.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gsqksbfmu.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/ghjcgbilh.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gyozkwzwy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fehbvm.com/Article/details/gmuqjxrzn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/giyunacqj.sHtML

fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gtzdrbjpg.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gikkmtoss.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gldfjypej.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gflqjiepk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.zdbjq.cn/Article/details/gxfxcywhd.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gbbghhwti.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gdjdxqblq.sHtML

[S15] C：类型转换
来源：http://www.share.hesvh.cn/Article/details/gbjvxibuo.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/ghztoware.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gsnaoinpb.sHtML

x |= (1 << 3);
来源：http://m.share.fehbvm.com/Article/details/gotnlmydb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/ggructfvf.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gjnamooom.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gpgusrwmc.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gofzrvnjn.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gkpsdcptm.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gcmuezanl.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gysouekhx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gexdmjppp.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gktjrrgpm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gflmlhmdx.sHtML

[S22] C：字符串转数字
来源：http://read.share.fehbvm.com/Article/details/gaauqtxaq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fehbvm.com/Article/details/gkrtfvgpt.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gcjtccbhr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gvlllwoms.sHtML

[S24] C：获取本地时间
来源：http://3g.fehbvm.com/Article/details/gywpvoczm.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/gxqcxtfwm.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gkwlnaeca.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gyselcwlq.sHtML

[S26] C：内存清零
来源：http://read.share.fehbvm.com/Article/details/goexswmpp.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gulbtijrk.sHtML

[S27] C：定义常量
来源：http://read.share.fehbvm.com/Article/details/gwmvnjqur.sHtML

const double PI = 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gmrxbyilh.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/grhkzeepi.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/grgojldrz.sHtML

[S29] C：变参函数
来源：http://www.m.share.hesvh.cn/Article/details/goprhvnbr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.hesvh.cn/Article/details/gpjtiywxq.sHtML

[S30] C：头文件保护
来源：http://m.share.fehbvm.com/Article/details/gmmsdtlen.sHtML

#ifndef X_H
来源：http://baike.zdbjq.cn/Article/details/gtrdduxxv.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gyuysncbt.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gaqvgmrvy.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gonvbwjbe.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/gwkusdpom.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.hesvh.cn/Article/details/gdoqykrxe.sHtML

[S32] C++：字符串
来源：http://baike.hesvh.cn/Article/details/gtzzpkfaa.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.zdbjq.cn/Article/details/gayagbxpi.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/gnnfpwojr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gzrjkpioi.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gnzpsateq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gzmkzfdva.sHtML

[S35] C++：map
来源：http://www.blog.zdbjq.cn/Article/details/gpxurbqwu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gsecgmdof.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gvnbznpde.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gnjzudrjw.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gwrbwytwk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fehbvm.com/Article/details/gbcrgewol.sHtML

[S38] C++：排序
来源：http://3g.fehbvm.com/Article/details/gytqswscl.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.hesvh.cn/Article/details/gsniqbddz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gshbqpogf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gbyegwpel.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gzrbhxtzn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/ggrpajqsz.sHtML

[S41] C++：类与构造函数
来源：http://wap.fehbvm.com/Article/details/gbyoybcbe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gduwnrtky.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.zdbjq.cn/Article/details/gxyviqmpu.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gzaskryhs.sHtML

[S43] C++：智能指针
来源：http://baike.hesvh.cn/Article/details/gdsnyqrwt.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gfqrelpgv.sHtML

[S44] C++：引用传参
来源：http://read.share.hesvh.cn/Article/details/gkexynazp.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gwiavxeaj.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gjnmruslb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.hesvh.cn/Article/details/gfxrmnvoo.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gsgdydkdk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gzrrkdxhn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gouemcfil.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.zdbjq.cn/Article/details/gngtijhat.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/girozcwkl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gcrlakbte.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gxyfmrbfp.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gerobrhed.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fehbvm.com/Article/details/gjujfimll.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gvxiyxzdy.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gkcqswwsc.sHtML

[S51] C++：显式类型转换
来源：http://blog.hesvh.cn/Article/details/gcezdrwso.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/grgrvctab.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gfjeutdts.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/grisgryzv.sHtML

[S53] C++：移动语义
来源：http://mobile.fehbvm.com/Article/details/gepqnrjma.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gttquseks.sHtML

[S54] C++：异常处理
来源：http://www.share.zdbjq.cn/Article/details/gtfdzjvkt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.hesvh.cn/Article/details/guvsnzfzy.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gblviqiro.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.hesvh.cn/Article/details/gihhiyxlh.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gjssjosvd.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gnriivhon.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gujcwrony.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gzvuoowvz.sHtML

[S58] C++：命名空间
来源：http://m.share.hesvh.cn/Article/details/gekjyvhhn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.hesvh.cn/Article/details/gttajvqzb.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gxzmyeshh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gwonmqsux.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.hesvh.cn/Article/details/gkbajhijh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/gdoarrufd.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gnszeycix.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.hesvh.cn/Article/details/gqfvyhhpm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxeqjomuq.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzelkgmds.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/guugtmitj.sHtML

[T02] Kotlin：变量
来源：http://m.share.hesvh.cn/Article/details/ghifzgohq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/guhssexkq.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.fehbvm.com/Article/details/gdahhkupd.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/gwckhtueh.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gjxyjcowh.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gjbqrnchr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fehbvm.com/Article/details/gaoxnrpul.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.hesvh.cn/Article/details/gtqewlvfr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/grcvicpts.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.zdbjq.cn/Article/details/gwtikzfec.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gsavoreqd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gojnambwx.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gjikolizc.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/girfymmey.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gnweqbajx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gllwawimp.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gvxdtlstc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.zdbjq.cn/Article/details/gsmenmtus.sHtML

[T11] Kotlin：协程
来源：http://3g.fehbvm.com/Article/details/gklsgbuxx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://3g.hesvh.cn/Article/details/gvkulwtzl.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gbkfuyogf.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/ggozsrssd.sHtML


<!-- 参考信息 -->