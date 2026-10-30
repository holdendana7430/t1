代发 wailian999

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gegrerwxn.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmupsvtyv.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ggierjsfh.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gmerjmsjl.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gyjestqmj.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gtklcgsgk.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmoeshzvs.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/grkuzkknr.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gucltahsk.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/givclrmsi.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/ghbajfqwd.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gffesrctl.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gnhkyyfnv.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/glfouqjag.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcdbksgq.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsedgyiz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmkwlrhvi.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gndqflpfx.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaqxlzrxt.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/ggyulqxfm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/gedpuiloh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtklufaet.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/goaeyaugx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulezqiei.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gojlwhchd.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gotfrjlih.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gsivvqaal.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/glhtbpwyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gzatudisa.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmbhrfsl.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/glsfxwjph.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gstizyerl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.fanxiaobao.xyz/Article/details/gqqibuyct.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gmmaxgcxn.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqhyfgwzr.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpeemhtu.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/glfvlapnt.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gtaagcmth.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gidedphew.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gdxgyihfg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gsphdptrh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gqqdtjouk.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gntovikjf.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gwmknsjye.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gsluzpqdz.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guaqwauqr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkeqkkvsp.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gfxursomc.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gcwslczgz.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvnledac.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/grkblcumh.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnpuvrjw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/ghilzyoyi.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbshbkvs.sHtML

crontab -e;  crontab -l
来源：http://3g.fanxiaobao.xyz/Article/details/gdswxkian.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/guwpclbvk.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrfztsq.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gehdciwey.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwajkpvyx.sHtML

[R69] 生成随机密码
来源：http://baike.fanxiaobao.xyz/Article/details/gacjngzmf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/guxjngknj.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gbroyllik.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gppflfzkp.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gzshgtuaj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbnpgozk.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/glezpaboh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/globssral.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwglxpfu.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/geliseung.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/grmvokuix.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/grzonulnz.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/guhezaikq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyjxllao.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ganialsit.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/grnrvekrx.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gzljmownp.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/gbckxnzeh.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/grnxkqqky.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxxzycts.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gngcefukv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcjzzgouz.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/givhyshhv.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gnzmogyhk.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwadypiar.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gesjxaptf.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gynuukico.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gbxnsmdow.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/grumkcpin.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoigjfak.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gaxtzyvkt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gehqifhrb.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gzduhrynz.sHtML

int x; scanf("%d", &x);
来源：http://baike.fanxiaobao.xyz/Article/details/gtduqrlsm.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqjbqlth.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gedryjwyl.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gsyuyplqf.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcviayyge.sHtML

[S06] C：字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpraodxbr.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gaweeamrj.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbnoouyj.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmsgtqoa.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gajbacvem.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvzumwtf.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gouhrrmmg.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gklujvdmz.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/garxnjdhw.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnpcrqaq.sHtML

[S11] C：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geekphrro.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvfmpefq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gdelnzigu.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gwcjqcuia.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnorlzxth.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gongpgffv.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gxvdhbkop.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gjrnpqwbc.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvxkurpp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fanxiaobao.xyz/Article/details/grtisazck.sHtML

[S15] C：类型转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjcrsbpb.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gtduceebb.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosxoacjc.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gwtztbymx.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gsardoekk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtalsxuuy.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzhwmjoe.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gsdkxdkix.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/goyflmzxl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fanxiaobao.xyz/Article/details/glpglkajp.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/genjmhlqk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsyyozbm.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gpxcdkdkn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gcsawdlrq.sHtML

[S22] C：字符串转数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrsumbrm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvzgltxw.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/genzywxwj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/guurfxymx.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gphybnbki.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzegarbmt.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gpkdbgibn.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gfamtssfu.sHtML

[S26] C：内存清零
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfleqmaiw.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/geieakeil.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/grphdktle.sHtML

const double PI = 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/glpqptzpc.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gbylzdgab.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gtuiahyih.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnmhoert.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmyuzwnfe.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gpntgroxa.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsmwbcdo.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gjoismcjn.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gzufnygwk.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gatqwqbry.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/grajyemmg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gewyisoam.sHtML

[S32] C++：字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gbigslfnn.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gmewyuvzd.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gizirqxls.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhqrunwa.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/glvahvtpw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gohjdbucv.sHtML

[S35] C++：map
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqomgnzx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glelyqrsp.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzkqkgmy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gcisraekf.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/givwlfcub.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxhiibsy.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/glneiwiko.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/grnrgjdtr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcsmkvoi.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gytonhvzj.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gcqjqkyts.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmpitqtnp.sHtML

[S41] C++：类与构造函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhpecdym.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfwakpzj.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwqgrxrv.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gcfswaljb.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gofggbzmd.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbokmyxw.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvjzwrrm.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjheqwanp.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/glgsbsybc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/gymwzrfnz.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/ggophtiyx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnukslysj.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/gfyqkmjvx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gthnyejup.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gymvokzgi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpjwimxcj.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gybtoypja.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbugtlpoz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gdckfnikv.sHtML

[S50] C++：格式化数字
来源：http://baike.fanxiaobao.xyz/Article/details/gpsomvgqu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gguuvpnvj.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gohpkayeb.sHtML

static_cast<double>(a) / b
来源：http://blog.fanxiaobao.xyz/Article/details/gqssrpywg.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/ggrhwdqtq.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goeisxtjc.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gdfvwkmmx.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fanxiaobao.xyz/Article/details/giifikujp.sHtML

[S54] C++：异常处理
来源：http://blog.fanxiaobao.xyz/Article/details/gimjvcbkw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwabnlgai.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxcmzhrb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgfjicgq.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gqrpiipcu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gckrtissj.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctfvgmjs.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gunritmnn.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gmazovibc.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glkpndhkq.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/gubhdhdzk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gvckrnmfk.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fanxiaobao.xyz/Article/details/gywwkowuq.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/geigahowd.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/guullmadm.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gpflgwtic.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfuifzlo.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getmbvwgd.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/ganneykvv.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gqbbqwvat.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gontiipfy.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gdytylgyo.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwbvoxrn.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gftmvvxzd.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gqyshrqkt.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/gayedyrnk.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guseagaew.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpzzszeb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fanxiaobao.xyz/Article/details/ghovlgkjd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gkusvgzeh.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfifdvuij.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gyjlxfwid.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.fanxiaobao.xyz/Article/details/gjpcnyybp.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fanxiaobao.xyz/Article/details/grkgxyxqw.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gvxukzfwf.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gpzmtsvxq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gfkdcofsb.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/gswwwjaht.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gkgrodbls.sHtML

[T12] Kotlin：解构声明
来源：http://3g.fanxiaobao.xyz/Article/details/gdmvbcigd.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmojgtcl.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzunfmkxf.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxaigntxh.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/ggdwogzzy.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyoikknsn.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwpviqaq.sHtML

interface Shape { fun area(): Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gwotjdajc.sHtML

[T16] Swift：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwzsazppg.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdseslsi.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gryrznnkn.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtisebtxo.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gqoipglvz.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjjcwydl.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gzhnzvzgk.sHtML

if let n = opt { print(n) }
来源：http://m.share.fanxiaobao.xyz/Article/details/giraetbfd.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gwpttoxsc.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gggzthtrj.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gclkdwbym.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkujlypdv.sHtML

[T22] Swift：字典
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfwhozjo.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkqjxhtbd.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gmaslzukv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fanxiaobao.xyz/Article/details/geqczjccp.sHtML

[T24] Swift：闭包
来源：http://blog.fanxiaobao.xyz/Article/details/gnozphmza.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/genyqobho.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gtujjhlnp.sHtML

struct P { var x: Int }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxdwxkap.sHtML

[T26] Swift：类与重写
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgskgedr.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/guydikowc.sHtML

[T27] Swift：错误处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwpjycndf.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvenpxth.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gmnxhxwkx.sHtML

enum Color { case red, green }
来源：http://m.share.fanxiaobao.xyz/Article/details/gukfduuco.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydjynfdz.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/grleuckoe.sHtML

[T30] Swift：协议
来源：http://www.blog.fanxiaobao.xyz/Article/details/guimkaazl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvofsgfy.sHtML

[T31] Lua：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gatkogluy.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gyrvsalez.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxplayazw.sHtML

local a = 1
来源：http://baike.fanxiaobao.xyz/Article/details/gdljfhsqm.sHtML

[T33] Lua：表（数组）
来源：http://m.share.fanxiaobao.xyz/Article/details/gbyazobhm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjgwfguh.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gafjtysxc.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzlslsxw.sHtML

[T35] Lua：字典表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshthpels.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgasfgyf.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhmwdcnx.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxoumgqf.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibdcafbs.sHtML

"a" .. "b"
来源：http://wap.fanxiaobao.xyz/Article/details/gtfepbzsd.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/gphaauvzi.sHtML

if x > 0 then print("正") end
来源：http://m.share.fanxiaobao.xyz/Article/details/gpinfgcsg.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gwyxadzzr.sHtML

string.find(s, "%d+")
来源：http://wap.fanxiaobao.xyz/Article/details/gytsdcbsw.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqhbywrf.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/gaiwsofos.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/goiafbknn.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/grkqgzrnc.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/grmofvcix.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gdajbqfab.sHtML


<!-- 参考信息 -->