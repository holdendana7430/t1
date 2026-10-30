代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gedsryhpz.sHtML

[R24] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gaynlkjnd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.zdbjq.cn/Article/details/gshagpbwi.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/grjprhaza.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.zdbjq.cn/Article/details/gtlccfezb.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gerchmdhs.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gzqputjcx.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gttnbooxl.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gbcdusrcw.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gyfszmbje.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/glhdhtpqu.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gtrqqswqy.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/govsegwng.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/ghnymgxqi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gggbhosbw.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gmexthocy.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gonmglprq.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gjluezxtl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/guhcgofew.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gwbhatlhs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gueixiwyo.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/gruovknte.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gndpnqhhr.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gtarogarn.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gxgznicjg.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gysinlixk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.fehbvm.com/Article/details/gqiurwtap.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gmovoymih.sHtML

files=$(ls -1)
来源：http://www.blog.zdbjq.cn/Article/details/gcdghefli.sHtML

[R38] 管道串联
来源：http://baike.fehbvm.com/Article/details/gfyxhjqeo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gpmvmowtm.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/glcyfvtsj.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/gyvozvrxt.sHtML

[R40] 追加写日志
来源：http://baike.zdbjq.cn/Article/details/gfpzwxmld.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gasrejjfr.sHtML

[R41] 丢弃输出
来源：http://wap.fehbvm.com/Article/details/gcfpykhlt.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gphjpdepd.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gnelefifc.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gtxonfrbq.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gygsgkqff.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gcidcckwu.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gqcbmoong.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/ggznwqfrn.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gzvltvtzl.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/galcakgjg.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gswbolgmq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/ggpussfrp.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gxdhglilv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/gzcvatint.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/gpmyzgumb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gexeqmrlo.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/glpbvhesn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gqhwfiujp.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gwcncmrlg.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gvgpxxsdm.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gyeqjegoe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/gzesvapca.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/gxhtdmhcg.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gxpqgxzlh.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gfedhqfbc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gfmiogfnh.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gkhxlwmfw.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gfjglmgsh.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gnkdnmoxy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gpzkogecw.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gqrijsleg.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gmzzqrehr.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fehbvm.com/Article/details/gkeruqqrl.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gfibzvilz.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gpyxvmbes.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gegulelsc.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/ggxaueasv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gkncbkeyn.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gdwruyaef.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/geufzszni.sHtML

[R61] 磁盘占用
来源：http://blog.fehbvm.com/Article/details/gqxqzacyh.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gafagqizo.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghknkdekl.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gqvznqjih.sHtML

[R63] 内存与进程
来源：http://www.m.share.zdbjq.cn/Article/details/gdvvthotl.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gxpowbnmj.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gkzzahlem.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gnqyqtqnm.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gwqquvoxe.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fehbvm.com/Article/details/gwidzhtjb.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/garjrmlke.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gouhbfpjb.sHtML

[R67] 生成随机十六进制串
来源：http://wap.hesvh.cn/Article/details/gklycomzk.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/glqtisjea.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gunuhdvdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gdfqkcody.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/goegiaurx.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gghzjlcby.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gtqhosesy.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gixahzfgh.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gwvvrwuab.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/gldpgckec.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gxcsqacff.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gkeuocnic.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/glbzsjknz.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gupgczyoa.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gwxcjstkm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gynxvhgrf.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gfasxxinu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.zdbjq.cn/Article/details/gcoupexkc.sHtML

[R76] 使用临时文件
来源：http://www.m.share.zdbjq.cn/Article/details/guebzqqak.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gapsbpjac.sHtML

[R77] 读取用户输入
来源：http://www.blog.zdbjq.cn/Article/details/goxxutzfn.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gqdvkbjir.sHtML

[R78] 交互式菜单
来源：http://read.share.fehbvm.com/Article/details/gkpathzqj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fehbvm.com/Article/details/grbaizdeg.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gvjbbaflk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.zdbjq.cn/Article/details/gxxhzjmme.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gipvbuvzq.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gagpitdde.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gnizwuxbx.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gxjcxinav.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ggbqxlfop.sHtML

[S01] C：Hello World
来源：http://baike.fehbvm.com/Article/details/gbjppxbjo.sHtML

#include <stdio.h>
来源：http://3g.hesvh.cn/Article/details/gpebpjnjk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.hesvh.cn/Article/details/gbiewhvzl.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gaarvbegr.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gnqgcakie.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gxlazplbt.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gfphkzxqv.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gqanhsbls.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fehbvm.com/Article/details/gbtvfdkuf.sHtML

[S05] C：字符串长度
来源：http://wap.zdbjq.cn/Article/details/gggzoages.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/guhhgxxcb.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gfasvpowk.sHtML

strcmp(a, b) == 0
来源：http://blog.hesvh.cn/Article/details/guycywiuc.sHtML

[S07] C：数组遍历求和
来源：http://wap.fehbvm.com/Article/details/gqcfnprta.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gpxcqkrzm.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.hesvh.cn/Article/details/gmtmknlfy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gxweytxet.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gsmmcogqi.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/guhxstxjs.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/glxxtwphe.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gemefqmdl.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/glybufvxq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/gkumyroiu.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gmstxcclo.sHtML

fclose(f);
来源：http://www.m.share.zdbjq.cn/Article/details/ggxgdlcni.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gdynhrmxu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.hesvh.cn/Article/details/gungkqkoz.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gcqxcgaft.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/grpvazxyy.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gmlpciyaj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gytwmqgpt.sHtML

[S15] C：类型转换
来源：http://wap.hesvh.cn/Article/details/gpddwojlv.sHtML

(double) a / b
来源：http://blog.fehbvm.com/Article/details/gboawhysb.sHtML

[S16] C：位操作置位
来源：http://m.share.fehbvm.com/Article/details/gbtkubshb.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gvhzwrupk.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gppuondnv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gnqmycynp.sHtML

[S18] C：命令行参数
来源：http://baike.zdbjq.cn/Article/details/ggqujotim.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gikmvmkye.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/giydtkitv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gvgpdiltq.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gijfumhva.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gwxlgpgyv.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gylqiruki.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gtxstnsge.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gcxucjwue.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.zdbjq.cn/Article/details/gcaobocdl.sHtML

[S23] C：随机数
来源：http://www.blog.hesvh.cn/Article/details/gqumlicjd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fehbvm.com/Article/details/gltumeztp.sHtML

[S24] C：获取本地时间
来源：http://m.share.fehbvm.com/Article/details/gklmekpdh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fehbvm.com/Article/details/gfkbrloqq.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gylumefzz.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gsyldzsoc.sHtML

[S26] C：内存清零
来源：http://m.share.zdbjq.cn/Article/details/gbcjplazp.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.fehbvm.com/Article/details/gmunkxtcq.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gnndkgjbc.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfsbahnbw.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gyfgxpovd.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gxvrabiry.sHtML

[S29] C：变参函数
来源：http://m.share.fehbvm.com/Article/details/gvnklgvmv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gwippdbla.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gmpyhhipa.sHtML

#ifndef X_H
来源：http://baike.hesvh.cn/Article/details/gkvpptmta.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gvodqduju.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gtpeclveb.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gllhbpgqh.sHtML

#include <iostream>
来源：http://www.m.share.zdbjq.cn/Article/details/gyixwvfhz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gnsuomcxt.sHtML

[S32] C++：字符串
来源：http://3g.fehbvm.com/Article/details/gsdxbihus.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fehbvm.com/Article/details/gquvxoidk.sHtML

[S33] C++：vector 增删
来源：http://mobile.fehbvm.com/Article/details/gwrsermwf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.zdbjq.cn/Article/details/geigclili.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.hesvh.cn/Article/details/guuhgxrey.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.fehbvm.com/Article/details/gndeazkay.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gvtunvtlv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gjathxpfk.sHtML

[S36] C++：unordered_map
来源：http://blog.hesvh.cn/Article/details/gompiztbm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gcmsovqle.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gjyopqbbn.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/glqhhaqja.sHtML

[S38] C++：排序
来源：http://wap.fehbvm.com/Article/details/ggrzmuafx.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gkvmaoppu.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gyidflsxp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fehbvm.com/Article/details/gfikaliar.sHtML

[S40] C++：查找元素
来源：http://blog.fehbvm.com/Article/details/gohzhqwvf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wap.zdbjq.cn/Article/details/gibiskshe.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gbeejypke.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gktvpakbp.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/ghvijcxno.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/ghefucqgl.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gsvqljrjr.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.hesvh.cn/Article/details/gmdatmgdx.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/ghrnurvmu.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gxqnxwwxc.sHtML

[S45] C++：lambda
来源：http://wap.zdbjq.cn/Article/details/gwwlkccnz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.zdbjq.cn/Article/details/gverxfzxe.sHtML

[S46] C++：函数模板
来源：http://www.m.share.zdbjq.cn/Article/details/glvlklkdn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gcrjsgtnp.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gnccrumfw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.hesvh.cn/Article/details/gelnjndwt.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gdfczmetx.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fehbvm.com/Article/details/gllbidtba.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqcecwcbk.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gmhhsxkst.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.fehbvm.com/Article/details/gopggmvnh.sHtML

[S50] C++：格式化数字
来源：http://read.share.zdbjq.cn/Article/details/gdsnwglzr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gixzijoat.sHtML

[S51] C++：显式类型转换
来源：http://wap.fehbvm.com/Article/details/gpqyvtxfj.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/goxjxekew.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gfrswykwd.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gzvinkewt.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gpsnnbvmc.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.hesvh.cn/Article/details/gyybvtkub.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gtfwhogsj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.fehbvm.com/Article/details/gwavwotwp.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gykoptvuj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gwhovtaed.sHtML

[S56] C++：optional
来源：http://mobile.hesvh.cn/Article/details/gradrtztc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.zdbjq.cn/Article/details/gzbxgpvhq.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gfowuoqxd.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gbwrxorss.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gmuantlth.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gcdpjtfyo.sHtML

[S59] C++：静态断言
来源：http://www.blog.fehbvm.com/Article/details/guouoqwbo.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gwdoksaxr.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gtozljlvb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gbwyopbqu.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdqufyfaa.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fehbvm.com/Article/details/gimfdxwxr.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/glnixbqev.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gfritepar.sHtML

println("Hello")
来源：http://mobile.hesvh.cn/Article/details/ggbkffqeo.sHtML

[T02] Kotlin：变量
来源：http://wap.zdbjq.cn/Article/details/gtfzmlepw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gbjlokams.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fehbvm.com/Article/details/ghyqxufli.sHtML

"值: $b"
来源：http://blog.fehbvm.com/Article/details/geshouslj.sHtML

[T04] Kotlin：空安全
来源：http://m.share.hesvh.cn/Article/details/gokjarabt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/grtcdxssf.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gqclhahmv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/gwolhekzz.sHtML

[T06] Kotlin：集合映射
来源：http://3g.hesvh.cn/Article/details/gdpexwvlb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/grkzhohwm.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.zdbjq.cn/Article/details/gpgbgplil.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/gwtvooaro.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gnisudjpj.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fehbvm.com/Article/details/gdcheaayx.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/gyltetdop.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/ghczqhtug.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.hesvh.cn/Article/details/gyjtabzeg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fehbvm.com/Article/details/gonlugyqs.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/gznvevjad.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.hesvh.cn/Article/details/gacmbbgst.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gwcjsdozu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gpviagydj.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/giinnvrtz.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.zdbjq.cn/Article/details/gfuawnugf.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/grghqakwt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gikufntme.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gvrdvreul.sHtML

interface Shape { fun area(): Double }
来源：http://blog.fehbvm.com/Article/details/gdiuuvlje.sHtML

[T16] Swift：Hello World
来源：http://blog.zdbjq.cn/Article/details/gnxkxwlom.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gnegueckf.sHtML

[T17] Swift：变量与常量
来源：http://www.share.zdbjq.cn/Article/details/gkviejdcr.sHtML

var a = 1;  let b = 2
来源：http://baike.zdbjq.cn/Article/details/gthnljaas.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gjzutoklm.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gbqyvmudc.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gsoqdfqty.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gfwnffufd.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/glotnvvwb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gdcsxcfez.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gytrojkan.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gpvbjpmyt.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gmsgpglwk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gmawenlub.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gmsxixvlk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.zdbjq.cn/Article/details/gawiovwxv.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gyzrqijgr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gucktncxr.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/gxokpkdvg.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gfbckdocz.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gguwrnlze.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gdjlbkrou.sHtML


<!-- 参考信息 -->