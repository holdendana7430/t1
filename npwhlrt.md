代发 wailian999

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/ggvyncuio.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gtmsnyxnx.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/guxbzccje.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/gyxuyjdjv.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/geuhmomsg.sHtML

[R42] 输入重定向
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfvsemtt.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrpytmqj.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjucvzujc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpmihgio.sHtML

[R44] 按修改时间查找
来源：http://wap.fanxiaobao.xyz/Article/details/gloexoyba.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxwzetlgg.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gyhzgbytz.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/glpbgcqmb.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gwnhqzrhq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gfouuqnrr.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gauocmblj.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gpoebisxd.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnbzkzmo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzakeromo.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpcpinup.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzxvovdr.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gyxslvxzz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gbfhqppsg.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gbiwynypj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gwoiilchg.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gpeuyinil.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwbozrhlo.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gngysbljc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gfoqcfzyz.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gawurhabw.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gddfqplza.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gieexslud.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoqevyrn.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbthhjbs.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhvajqrl.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxdlfiyn.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/ggzhkbgrf.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gkciiyszq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gpigapfru.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gaaxxrgsy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grkanbzti.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/giaykobex.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gduafiouf.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/grczaqnza.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/glmqymapk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/goyjeifbp.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gqbmtfltj.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/ggfjxcsdb.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/grkaigikz.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gebfpmchc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomifospb.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbgregwp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gszgaztur.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gryfjfaod.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwlivocu.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwaonfco.sHtML

openssl rand -hex 16
来源：http://wap.fanxiaobao.xyz/Article/details/getcajioh.sHtML

[R68] 计算文件校验值
来源：http://blog.fanxiaobao.xyz/Article/details/gksxbcaor.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaascxyq.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/gszpepnff.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/gdiulamnd.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gsefyltlz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gpmpllaox.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gruobdqpg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcduuzoa.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gqawlerpd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlgnybek.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gpudlwvdd.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjqreppm.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gibhiynyc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghtitsauq.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/gbqoxavus.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwccwnek.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gqawpjdyn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gynxotjpq.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gcjtckkmu.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/gzwpaubgo.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/grzkwolpj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhawevpe.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gewixaamx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzprtwndv.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gxfzccfxl.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvskmrpmq.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gjncddega.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/glyxdnxqs.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjocrirn.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhvlmsyq.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gfatndtww.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/grazovuhm.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fanxiaobao.xyz/Article/details/gfwubtcwg.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/gocuxvskf.sHtML

[S03] C：读入整数
来源：http://read.share.fanxiaobao.xyz/Article/details/gjciokqqm.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gklpotrzr.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gyxwgvzah.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtpdoiepa.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ginmggjta.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/ggmlwugkx.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/grprpagwe.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/glghoalow.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/glcosmbde.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gfpyhnsqp.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gxxcxaqhe.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gndsciljm.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gkvvdtdyf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fanxiaobao.xyz/Article/details/gymmwywpf.sHtML

[S10] C：指针与解引用
来源：http://blog.fanxiaobao.xyz/Article/details/griylqcfp.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gliugmrfq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpndjcbiw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnvomwnh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gctxpegth.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyskfbki.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfatcjpwj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotifbwak.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggibibzdu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gygnoccfz.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqipbnwi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fanxiaobao.xyz/Article/details/gmidgnsve.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwrnrjuq.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsocvixjb.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gnibupgdw.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/guepdlogb.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssomxxhg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/glxtmtpug.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gpvvhzulw.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gphehifum.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhitzxef.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/guyxreerc.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkwuatte.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guigcaqyp.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/geuicplha.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxywyfkv.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/ghosvquvt.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gexgryssz.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyylxbwsm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/glcilrujb.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gvnmoipih.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqsrlsnu.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/gudqfqwyk.sHtML

memcpy(dst, src, n);
来源：http://baike.fanxiaobao.xyz/Article/details/gvwvcbihc.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gywgaorae.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvtxnjlcu.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxgqchqp.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gblulcncg.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/geuulnomi.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gztyzjhck.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gizjnjopc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwolimohb.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqbhkrom.sHtML

#ifndef X_H
来源：http://mobile.fanxiaobao.xyz/Article/details/glciodash.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpqlnbey.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqgeiyyz.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayvvfyan.sHtML

#include <iostream>
来源：http://baike.fanxiaobao.xyz/Article/details/gledyrbxq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gphlvcvvo.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbmyfkmw.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/ghtelllna.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwfcjqda.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugafmacb.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugbrkjzf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/guhgafnhs.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gitqdacku.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznacsjhe.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gajuigese.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbfeitnrz.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gfklizcgv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvplechh.sHtML

[S38] C++：排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gbliqbzps.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvnimttc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmltvbgx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fanxiaobao.xyz/Article/details/gsjoosgni.sHtML

[S40] C++：查找元素
来源：http://baike.fanxiaobao.xyz/Article/details/gkvaaxgpu.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giahrnvim.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbhmmyfp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gedmzleli.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/guuijwlfx.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbewwqqz.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gdtjdsmgt.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/gimrqarin.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gwqxninrf.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gebakyrac.sHtML

[S45] C++：lambda
来源：http://baike.fanxiaobao.xyz/Article/details/gjrephmbi.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/gcceibgyb.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqylkqgpk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmehodkto.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gqvwfnxui.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gaqsywnwp.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvrairtvj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtziudtge.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkukrmzle.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/ghwpfgoob.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fanxiaobao.xyz/Article/details/gekuxrqun.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwontcdm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/ghtmhufos.sHtML

[S51] C++：显式类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gppmfopln.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gnoonlebq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzdqhvghd.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaosjlwu.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gihfsbutu.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/grmybgjsh.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsevlahmk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gwpwvupjm.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctawqhdq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gheaqlgfo.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gbdbhkhry.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/goedqxvnw.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gjlbglkoy.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gpjkxdbxx.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gxxlqjmwj.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gbiohjihg.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gigueddap.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gehbqspea.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/grnfhaquj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxoaujzpr.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gfvlkhkti.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/grusqzrps.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzocdhzkk.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gcdgffizo.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigxgjgi.sHtML

[T02] Kotlin：变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkrrbqhs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmczthda.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gqaaxvqxc.sHtML

"值: $b"
来源：http://baike.fanxiaobao.xyz/Article/details/gwibnpouj.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/graqacnef.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fanxiaobao.xyz/Article/details/glicloenh.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gijszkhru.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcwgsxqn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqyqtmmql.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/gripwsfyc.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyhozhwy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gtzhpbwxv.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/gmmafpoai.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gbaylfthn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxrdaksq.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxzmhnwa.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemyedvhw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/grkimxcfw.sHtML

[T11] Kotlin：协程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsknanqq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkbteyct.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gerkmmkvr.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrmyvxwg.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.fanxiaobao.xyz/Article/details/gplbvfyht.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtexkkasn.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrobeuom.sHtML

for (i in 1..10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggvaabrci.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqzalrgal.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gsxzqqjqi.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgnmdupv.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gjnpykzva.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvaqaord.sHtML

var a = 1;  let b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gruabmhsh.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcgsaqln.sHtML

"值: \(b)"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxyjvkri.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcwofjrv.sHtML

if let n = opt { print(n) }
来源：http://3g.fanxiaobao.xyz/Article/details/gurbmhzrg.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrsendqy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.fanxiaobao.xyz/Article/details/gucrbewbx.sHtML

[T21] Swift：遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gohppdipt.sHtML

for x in a { print(x) }
来源：http://blog.fanxiaobao.xyz/Article/details/gctwncild.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicahzygk.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gxxglurfq.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gvfuousar.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwmitsbwk.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqvywcbs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlowzegd.sHtML

[T25] Swift：结构体
来源：http://wap.fanxiaobao.xyz/Article/details/gtwfcnyfq.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/ggefxlwqj.sHtML

[T26] Swift：类与重写
来源：http://mobile.fanxiaobao.xyz/Article/details/gsekjrwaq.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gfztdrqhf.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/ghjparkno.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fanxiaobao.xyz/Article/details/gmknjmnxb.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/ggjosymqz.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzoyimtop.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcyngiit.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsizwbknn.sHtML

[T30] Swift：协议
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpyauhch.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/gribqjkff.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gjlxfbdax.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxsocygu.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gpftpscnk.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmkclpfu.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/glxnwcjvq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gbmwogymx.sHtML

[T34] Lua：遍历表
来源：http://blog.fanxiaobao.xyz/Article/details/gzjtsyqrb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gnodhiuci.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdqnwgbk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.fanxiaobao.xyz/Article/details/gwglsjnox.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxglurei.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gmymhpuud.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/golugfmiy.sHtML

"a" .. "b"
来源：http://baike.fanxiaobao.xyz/Article/details/gvxtibnac.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtgvqqlfx.sHtML

if x > 0 then print("正") end
来源：http://3g.fanxiaobao.xyz/Article/details/gjyeejbwy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwmidfkm.sHtML

string.find(s, "%d+")
来源：http://blog.fanxiaobao.xyz/Article/details/gqvlhxmai.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grodahqym.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyflblcc.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozwsnpnd.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/ggqkurpvq.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gqtpdkxwu.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fanxiaobao.xyz/Article/details/gasmshjgt.sHtML


<!-- 参考信息 -->