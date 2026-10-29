代发 wailian999

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/gbxdzvsid.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gzddmehyg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gzshezded.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gefjdyzxj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/grssuxjca.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gtypfvuqr.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gpxqjemdr.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gqwgpdgxq.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gxcaccpec.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/grzcoieup.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gdrmmnhht.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gnrlbmltu.sHtML

cmd > out.log 2>&1
来源：http://baike.fehbvm.com/Article/details/gbnhxkdev.sHtML

[R40] 追加写日志
来源：http://3g.fehbvm.com/Article/details/gizzgulkt.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gcnmlgcxk.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gbufsbhue.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.hesvh.cn/Article/details/geingouur.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/glpzqnmfh.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gptdoaunj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcmkyessa.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/guzzgynym.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/gnlifaglp.sHtML

find . -mtime -7 -type f
来源：http://baike.fehbvm.com/Article/details/gvyinqlvw.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gnuwaaqni.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gpscdhywy.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/glwhxdleu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/gqmsgvqrx.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gtoboolob.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gykvicbln.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gismngcax.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gjrnqhbfi.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gmwhzumlq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/gynghgblv.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/gvldcgtwz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gtqmuwcwb.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gsjjvwvaj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.zdbjq.cn/Article/details/gsjufdrih.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gkxmdiqeo.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gwremrfnr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gzejfxigy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gxrpgwwns.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gdlaglclo.sHtML

diff a.txt b.txt
来源：http://www.blog.hesvh.cn/Article/details/gqsbreyvt.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gocnkntyo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gezhagdhf.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gyksqqkku.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gyudneaqr.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gfodveocv.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/gorfczlms.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gcbbwtyfg.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gsxhvrdpn.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gpfdrankh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.hesvh.cn/Article/details/goiqqmmbj.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gcwwvvkjt.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/goasctrap.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/goihpsgnp.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gguvgbfxv.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gxywbjqgy.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gorekncrk.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gmcigzzop.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.hesvh.cn/Article/details/gfdbwzysz.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/grknzvhno.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gqgzpzsea.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gclthnvaf.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gknrqfxwt.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gclskplra.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/ganivxpuq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/ggekbqjnh.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gcbuodszn.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ggikjhxvg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/geqwmxxjg.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gnetftuht.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gelvgnhza.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/ghmslaefl.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gitnlbdam.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gatxiumdo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gimnzcmai.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gcowxmkts.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gzmsgqjum.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gpwgcrauw.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gnbgffyol.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gosdagrgw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/glxismrzh.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gcapvdjfj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/ggoznpzvc.sHtML

[R76] 使用临时文件
来源：http://blog.fehbvm.com/Article/details/gmybovagk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gmhzdtjvo.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/galolsued.sHtML

read -rp "请输入: " ans
来源：http://m.share.zdbjq.cn/Article/details/gvlvndnrm.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gsuaohvym.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gbynpfrpw.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gtvfoqwmb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gpgoarixq.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fehbvm.com/Article/details/gnoofdjbx.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/garxhxdis.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gptspjzrd.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/grqkminut.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gythufjxj.sHtML

[S01] C：Hello World
来源：http://www.share.fehbvm.com/Article/details/gazivpifc.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/gbayczonm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gscpqxxnb.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fehbvm.com/Article/details/gbhpysypa.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.hesvh.cn/Article/details/gqfalcjxc.sHtML

[S03] C：读入整数
来源：http://www.share.zdbjq.cn/Article/details/gznnobyji.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fehbvm.com/Article/details/gikcypbrk.sHtML

[S04] C：字符串复制
来源：http://blog.hesvh.cn/Article/details/gdwisrorv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gdylcunfd.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gdkylyzbc.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gnadxvbkt.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gdorbfkzy.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/gytnzvffq.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/gkihagdrf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.hesvh.cn/Article/details/glzgjvgcg.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.hesvh.cn/Article/details/gbwvjixrs.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/gzskheudg.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gpoplnnjb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gmjowsklt.sHtML

[S10] C：指针与解引用
来源：http://www.blog.zdbjq.cn/Article/details/gwdrkyctv.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.hesvh.cn/Article/details/gqtbjvlns.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gnfiorump.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/gjhsziofa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gwuryykxq.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gkagzbdhe.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gtymmukly.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gwouxmofo.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/ghiwsmcma.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.zdbjq.cn/Article/details/gxqisbxqi.sHtML

[S14] C：枚举
来源：http://mobile.hesvh.cn/Article/details/gqdchnohp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gumemcokj.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/glqewtewc.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gerrqtuvw.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gsdxnqouz.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gweklndvv.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gkpbkqhwk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fehbvm.com/Article/details/gtvovheeu.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gzgybgizs.sHtML

int main(int argc, char **argv)
来源：http://wap.hesvh.cn/Article/details/glsvcoxbg.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/giumvfgsh.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.hesvh.cn/Article/details/gkheoqhia.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gouegowlq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ghoqlsnei.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.fehbvm.com/Article/details/gwyemiwvq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gmjoaibvn.sHtML

[S22] C：字符串转数字
来源：http://m.share.zdbjq.cn/Article/details/gdfdksece.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gwccwehwa.sHtML

[S23] C：随机数
来源：http://blog.hesvh.cn/Article/details/gbtbznjzo.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/geejajaua.sHtML

[S24] C：获取本地时间
来源：http://www.share.hesvh.cn/Article/details/gvqslytzo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gcyzulnvp.sHtML

[S25] C：内存拷贝
来源：http://blog.zdbjq.cn/Article/details/gzitajbwj.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gtknzacsx.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/givjnhiud.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gclspmsfl.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/gqbddrupp.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gepwojkty.sHtML

[S28] C：静态变量
来源：http://www.share.zdbjq.cn/Article/details/gfisuuqra.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gxrrxfczi.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gdncvrssx.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/gankxtbke.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/gvlsjcmuw.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/ghawrypvk.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gxyumhoej.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gdhrtkdvb.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gaththkxm.sHtML

#include <iostream>
来源：http://mobile.hesvh.cn/Article/details/gwfuyhcft.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fehbvm.com/Article/details/gipzrtgnx.sHtML

[S32] C++：字符串
来源：http://www.m.share.fehbvm.com/Article/details/gdepzfjfb.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/grlaimfxi.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/glpjdsonw.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gtnptndey.sHtML

[S34] C++：遍历 vector
来源：http://blog.zdbjq.cn/Article/details/gkqnhhvhy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.hesvh.cn/Article/details/gvjblpnqb.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gnqtdlmdl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnqrawveq.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/grlirubnq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gmkpwyunw.sHtML

[S37] C++：set
来源：http://3g.fehbvm.com/Article/details/gbjjqihqv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gltxpokpe.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gyfpivult.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gekblqlfm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/gofancwsw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gffysrbcq.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/gyandltwf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gjyhzkvjv.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/gsfhjilte.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/ggciflyij.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gnmimbhhg.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.hesvh.cn/Article/details/ghaaemhzq.sHtML

[S43] C++：智能指针
来源：http://read.share.fehbvm.com/Article/details/gjfdftrbn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gixgaijaw.sHtML

[S44] C++：引用传参
来源：http://www.share.zdbjq.cn/Article/details/gbmizwhrm.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fehbvm.com/Article/details/gpplxfijv.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/glvpoezkq.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.blog.zdbjq.cn/Article/details/gffpcauee.sHtML

[S46] C++：函数模板
来源：http://www.m.share.hesvh.cn/Article/details/goizshkpz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.hesvh.cn/Article/details/gxmkocktx.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.hesvh.cn/Article/details/gvgvglirr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fehbvm.com/Article/details/gxzewmdyj.sHtML

[S48] C++：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gxxdkpurj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gxsrltark.sHtML

while (std::getline(in, line)) { }
来源：http://www.m.share.hesvh.cn/Article/details/giqsfnhkj.sHtML

[S49] C++：写文件
来源：http://mobile.zdbjq.cn/Article/details/gvqfsbqgj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gqeejwuba.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gctqdclxd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/geownkvdr.sHtML

[S51] C++：显式类型转换
来源：http://m.share.zdbjq.cn/Article/details/gzympuvdp.sHtML

static_cast<double>(a) / b
来源：http://www.blog.hesvh.cn/Article/details/gmxjexvul.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fehbvm.com/Article/details/ghlvpmebx.sHtML

int size() const noexcept { return n_; }
来源：http://blog.hesvh.cn/Article/details/ggknvifub.sHtML

[S53] C++：移动语义
来源：http://3g.hesvh.cn/Article/details/gafbhorwh.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gdndsurru.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gciufcruy.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gyklyoiez.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fehbvm.com/Article/details/ghxnwbexw.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gigrqziij.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/glofaynbn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/gwlrbahbh.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/grpgwpqma.sHtML

constexpr int N = 10;
来源：http://www.m.share.zdbjq.cn/Article/details/gqoijvxez.sHtML

[S58] C++：命名空间
来源：http://www.share.fehbvm.com/Article/details/gstiwafks.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/ghojyzlrp.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gogxpnsyl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/ggkoozhuf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gdnphrxok.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.zdbjq.cn/Article/details/gtkgixhxq.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gyihvrssv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.hesvh.cn/Article/details/gzgdcwxrf.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ghcmquxad.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkornqjjy.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/gfeqikdpp.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/gdtikbudh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gmiwemldq.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.zdbjq.cn/Article/details/gksffregw.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gmukszibz.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/grvnzqtzb.sHtML

val n: String? = null;  n?.length
来源：http://mobile.zdbjq.cn/Article/details/gaakyenam.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.fehbvm.com/Article/details/gtkupnpno.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gifzyczbb.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gpvsjspvp.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/ghreggxjn.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.hesvh.cn/Article/details/gkrodkylg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gajfczqrv.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.hesvh.cn/Article/details/gwdrxeute.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.fehbvm.com/Article/details/gnxvwfltr.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gvvjhkfgt.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gwemtseop.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gbmkxpzin.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.zdbjq.cn/Article/details/gmbrrxypc.sHtML

[T11] Kotlin：协程
来源：http://wap.hesvh.cn/Article/details/gfkyxjjqr.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.zdbjq.cn/Article/details/gtdzygjyd.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fehbvm.com/Article/details/gicgfijcc.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/gtquazoqd.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.hesvh.cn/Article/details/gmcravjim.sHtML

val m = mapOf("a" to 1)
来源：http://baike.zdbjq.cn/Article/details/gbaggpfkg.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/glxowmyxa.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gksvuzvmf.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gijkfkbnx.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gugkslxxs.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gwvwhiksa.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gpfsbeuqi.sHtML

[T17] Swift：变量与常量
来源：http://wap.fehbvm.com/Article/details/gqjfmzepp.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gqfbbbtcq.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/gsbcqloeu.sHtML

"值: \(b)"
来源：http://3g.zdbjq.cn/Article/details/gtqdsfrqb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/grvnzckaz.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gjqwdxjqh.sHtML

[T20] Swift：数组操作
来源：http://3g.fehbvm.com/Article/details/gnutonmko.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gjkolplxh.sHtML

[T21] Swift：遍历
来源：http://baike.hesvh.cn/Article/details/ghzanwkmt.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/gjanvddhh.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/ggrhgperq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gdvhsohdj.sHtML

[T23] Swift：函数
来源：http://www.m.share.fehbvm.com/Article/details/grqieyqfj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gbovrhgeu.sHtML

[T24] Swift：闭包
来源：http://mobile.hesvh.cn/Article/details/ggensvmkj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/guwhhuvxx.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gpblpvaxe.sHtML

struct P { var x: Int }
来源：http://m.share.hesvh.cn/Article/details/grjhqoang.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gsrlxeval.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/grinzmztu.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gxkutcied.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.hesvh.cn/Article/details/gmyitzwqi.sHtML

[T28] Swift：枚举
来源：http://blog.hesvh.cn/Article/details/gilnbgtgw.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gouxczvue.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/geugfdlmr.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gvfshepoz.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/gnhiedmsx.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/glrxpmmic.sHtML

[T31] Lua：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gchjaqcbe.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/gobuyrowc.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gbxjchsxg.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gpwbylubl.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/giljkdmbz.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gbuliqbba.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gscmvkuxz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.zdbjq.cn/Article/details/gokpkteea.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/gqaofajkf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.zdbjq.cn/Article/details/gxvdurema.sHtML

[T36] Lua：函数
来源：http://wap.fehbvm.com/Article/details/getfeyrrf.sHtML

function add(a, b) return a + b end
来源：http://wap.zdbjq.cn/Article/details/gcjatxega.sHtML


<!-- 参考信息 -->