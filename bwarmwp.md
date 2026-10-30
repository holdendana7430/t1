代发 wailian999

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepfnxmcp.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnjmhtqkq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxlwqrby.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/grtyottky.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gonmwxjhe.sHtML

[R22] 截取子串
来源：http://blog.fanxiaobao.xyz/Article/details/gcfebvpor.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxqwwxko.sHtML

[R23] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxomvvtn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gowdwneah.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gpeyhdshv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxbuqusl.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gplwnakqv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gmtvffzgc.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckzhkbgf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fanxiaobao.xyz/Article/details/gyvdzuioj.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gvuzpilwy.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/guxgtabxr.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzctfngpz.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyuqyrgh.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvzkhypy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gtcyvsdez.sHtML

[R30] 函数返回状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvreenuau.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gukedbfqk.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtdkcasp.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gesdcwsut.sHtML

[R32] 参数个数校验
来源：http://baike.fanxiaobao.xyz/Article/details/gmnsgqwed.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gfycoxlod.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gnwftkucr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/grddvjuce.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzhnimzh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/glcsicqen.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpnoomdwi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fanxiaobao.xyz/Article/details/gyrbetkfh.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyozydoob.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/giydeuzby.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gbbcpjsug.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gedccdabb.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/gegirwvvz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goelfsllr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjcpkxrsp.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/grmfpjauy.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gjslecrcc.sHtML

echo "log" >> out.log
来源：http://wap.fanxiaobao.xyz/Article/details/ggjbxwbqg.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gedaqvabw.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gxfepdnew.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gpwsucrqd.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpyziokyi.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfnlkgxv.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gftknzfag.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/ggqkgsnyw.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geecmktte.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gkxiycgvt.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gxzfkezjp.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsimmjze.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjmhmvae.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gxicdzrpz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqqlvnyj.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gvyskthxp.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/galqmpgkl.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghrcgcopn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gpnorppzh.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gsdzsanzu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghgcopkxd.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjwvtgcm.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/ghzcvpxul.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gkswplajb.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcwktoid.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gaeqouncy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gnwpeilab.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/grrzeatal.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvfgplvis.sHtML

[R55] 压缩与解压
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrbmlwwr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/giqmdpauk.sHtML

[R56] 远程拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gvntakpth.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/goypdpzsc.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gvketpnii.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gzzzefalu.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcgqmjcj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gwaofrymw.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gpduligjg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gjuprenxu.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gpdatdqny.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/glvrteufk.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gttienpkv.sHtML

df -h;  du -sh *
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifzqwscl.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/golddfbvl.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gxygapszi.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsyooblb.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnyqprgm.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gqgfifmtt.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmsfeakiq.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvvuisai.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqosecict.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjirofkoy.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gazzoglaz.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsxgebrr.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gavhpkidr.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsvxjjgr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gpjyteeyl.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/ggsxhkydx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gjdkcvcta.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gbjucqibl.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gioayrywu.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/goskreejx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gnptywmvo.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gihwiikkn.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gndmnloid.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrffgtke.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkslafzlc.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcbxvrno.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvptxeqcz.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/glcdwoxto.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiqtonns.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmsnafzed.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gzoaawksm.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/glizevirj.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gzukcwwsu.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/ggswllmbz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmdphczu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumrpwrng.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gljcxarts.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziixtkou.sHtML

time ./run.sh
来源：http://read.share.fanxiaobao.xyz/Article/details/gijxpgunj.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkvipoebr.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gsvbvnbnq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfoyvfmum.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsqqufupm.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gzsxhcaxi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggapmzzlr.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gbexrdops.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqrhjmuqg.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsipwdjq.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gypbsvsao.sHtML

[S04] C：字符串复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/gezeupoea.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaonmmqb.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gdclhxwiw.sHtML

strlen(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gckewlulg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcflqahcx.sHtML

strcmp(a, b) == 0
来源：http://blog.fanxiaobao.xyz/Article/details/gwaomydyk.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxcucsid.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/giamqbdlr.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/guxvqmwvf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gnmqyxfsw.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gewendfhw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhjrtctg.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjspimwth.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gcqdejzdf.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsuhmcqwy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrrcwvqp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gzyvjjtzi.sHtML

fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ggncmssit.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghrxnovtp.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gspipmkht.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gntyrfhkd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gadtuphfz.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuvbdxng.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fanxiaobao.xyz/Article/details/ggreacens.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/goljuvmca.sHtML

(double) a / b
来源：http://blog.fanxiaobao.xyz/Article/details/gpaomzjms.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbnqvptj.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/glpogupwi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoqmgphd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gipbxgwnp.sHtML

[S18] C：命令行参数
来源：http://3g.fanxiaobao.xyz/Article/details/gtroiysdc.sHtML

int main(int argc, char **argv)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaeybymk.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gmlwccxnd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gxxgpjatd.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqilvvfp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/grixcqhqe.sHtML

[S21] C：字符类别判断
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgvqgvrq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/glkfsjeen.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/grdwpfsbi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbtosijc.sHtML

[S23] C：随机数
来源：http://baike.fanxiaobao.xyz/Article/details/gphlwvzin.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwobklfo.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnnolofs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gskiihpgk.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gingwdmtt.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzxzsybz.sHtML

[S26] C：内存清零
来源：http://3g.fanxiaobao.xyz/Article/details/gyrnqrxcy.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnoeobru.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutbhumko.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjmpsnkh.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslzuvnbg.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gamlhpdln.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfdfslwua.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fanxiaobao.xyz/Article/details/gezbakpvf.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gcofugcvi.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/goclfxbrp.sHtML

#define X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/garpuhiwm.sHtML

#endif
来源：http://3g.fanxiaobao.xyz/Article/details/gbyqgsqdf.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/goqhrmkfb.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwzbtdut.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvrrsnyi.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ggftktmyc.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphtdcipw.sHtML

[S33] C++：vector 增删
来源：http://blog.fanxiaobao.xyz/Article/details/gbxnltrpx.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gblrociwo.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznpsfrsb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gcznztcoc.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gpcvcrzbd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gqxbsaaeu.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gwxrqvygf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/glgohgucs.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gewbfkspd.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fanxiaobao.xyz/Article/details/grweiwbuk.sHtML

[S38] C++：排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guugbvfkg.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/ghjxlszwk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/grjjrembl.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gvukquocu.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxrtkcrd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmixjdoyk.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gibmfvqqg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqldqins.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gytowfbqz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvcyfbwa.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gxtziyucc.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuhveitz.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gzlyiqykg.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gimlynphj.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gdgxkdyfy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gzdzyhwta.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gqousjuoe.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbbhvhnz.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gjufrikct.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfdbmcfg.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geoqrzyta.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhortkjx.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqpxfrmvn.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghvehueqm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/gbqgizbri.sHtML

[S50] C++：格式化数字
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnbyhsql.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gkfyyunif.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gqevpbzsa.sHtML

static_cast<double>(a) / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvosiddmh.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gbsaswifm.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gkaewbzxz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhxyujnp.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqgdfktv.sHtML

[S54] C++：异常处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gftpjwqad.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpostilb.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssgcesuf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gixrxtrlb.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gbhhyrqwl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gpvyaqsae.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/glmmphvve.sHtML

constexpr int N = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrgyerwt.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gnoydxpzy.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/grxuefpoo.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiolgdwo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gfnabxfvu.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/ghgabinmu.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggrnqmzau.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gcopdnwsd.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gzywyfvka.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnvtmzcod.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/glajjgzin.sHtML

println("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqupoqgr.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gbkvjgvke.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigabdaln.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/ghigvebsy.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafehehur.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjxkapbx.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gceuzobst.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvusoualt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmlaqypf.sHtML

[T06] Kotlin：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/gnlrkjeen.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfssgibo.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gkyeozgke.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fanxiaobao.xyz/Article/details/gpxxjlaib.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifxhucva.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaegxgkwh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goopqhivy.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/ggpawclnw.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gaiblcwxk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/gitkbdavp.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyktxmmr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjkladrxq.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdvtsrwjh.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwkcldgg.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbifpdcs.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrhltiyu.sHtML

[T14] Kotlin：循环
来源：http://wap.fanxiaobao.xyz/Article/details/gikjyypog.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqbewcuv.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gdpgoflvp.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gjeazropz.sHtML

[T16] Swift：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gbazbbvhx.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gktuiatny.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/givfaitie.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gxtoqvmhi.sHtML

[T18] Swift：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gqssjqyby.sHtML

"值: \(b)"
来源：http://3g.fanxiaobao.xyz/Article/details/gcvdlmsws.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulcmvlek.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gamigjirt.sHtML

[T20] Swift：数组操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjuzwsubc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgsopefm.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gggosgqct.sHtML

for x in a { print(x) }
来源：http://wap.fanxiaobao.xyz/Article/details/gttwkmeyt.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gpussguzg.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gisaifnsc.sHtML


<!-- 参考信息 -->