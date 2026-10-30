代发 wailian999

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzmcpzkt.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcgbcclns.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/goeebztnh.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/grstqfdyk.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgeoxvvq.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwqzfxva.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpthddhcw.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gliurdsgs.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gqmcpxypo.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gkoookwbt.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwilugvq.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gnaajyggz.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fanxiaobao.xyz/Article/details/gehykzahd.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbboaqba.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gshqxfoah.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqdwgeoz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gvetwkkbs.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gfegnioap.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gkifqoxni.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gltnahalo.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gjvagamms.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gfjgprwut.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gjowywzza.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipcxiygr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyspmnvv.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gdxuvsbch.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelxyqqqi.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.fanxiaobao.xyz/Article/details/gkovofugs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbixurph.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbvohmrxs.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gncltfqnd.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gddocbyxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gfimnlues.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyuuvaptc.sHtML

scp file user@host:/path/
来源：http://read.share.fanxiaobao.xyz/Article/details/gwiothocz.sHtML

[R57] 远程执行命令
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsfmvtao.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gjfkrtoee.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gidhktbze.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gdrqhmdag.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbzrxwnb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/grxqrcwxy.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fanxiaobao.xyz/Article/details/ghsfsusah.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuynftuv.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gceeusswb.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gjazqfilg.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gxaphzwxb.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgyusrfc.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/grcmfnxnm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/ggaotvsiy.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gisoiogpl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxcyjars.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gmrhmajgw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqomsiwp.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gplymsegj.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gwivgsxfh.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjilreci.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadnzswel.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpjgwvajd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gmaauxnbi.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gtdntwxtd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gybhmnmnc.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gmwvqvnfp.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gzzeemjht.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gforflfbt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gtgvbhgxd.sHtML

[R72] 等待端口就绪
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyylcuvj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtjowlsfy.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/giqlsatke.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnipfdisw.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gdxhxezid.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgyywhel.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnaeyvwv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsljwjcam.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gojxmhdtd.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gabqtwnte.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsgxqkmt.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/getdbslws.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gkvmlmlma.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.fanxiaobao.xyz/Article/details/guqbttovr.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gkxtqqbiw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gddssytgj.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/gowjeyfuz.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqizxwtlc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gemphwzgm.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqxhizivq.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gkezeyuli.sHtML

[S01] C：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/grbuhcxvy.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gmizzhgws.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwmmyztjq.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncxpbmjt.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfqbxdkkw.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gxcqhbizp.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnoyrnro.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gubpvcyrj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.fanxiaobao.xyz/Article/details/gslcptkah.sHtML

[S05] C：字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gqpxnzbel.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdbulhjl.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gjcoikljz.sHtML

strcmp(a, b) == 0
来源：http://www.share.fanxiaobao.xyz/Article/details/grxilpyfk.sHtML

[S07] C：数组遍历求和
来源：http://wap.fanxiaobao.xyz/Article/details/ghodmcadw.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcskeplat.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gvzjpjgjd.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fanxiaobao.xyz/Article/details/gyphwafwy.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gkhrwknqf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhxofopg.sHtML

[S10] C：指针与解引用
来源：http://read.share.fanxiaobao.xyz/Article/details/gnanrjnfn.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gspsmgilh.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggimlkxdg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjpewqxv.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/geuarewfe.sHtML

fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuqqysad.sHtML

[S12] C：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrsrbgas.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/grpdwuiru.sHtML

[S13] C：宏定义
来源：http://baike.fanxiaobao.xyz/Article/details/gqurmfjvb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaakafswi.sHtML

[S14] C：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpvdsyenm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgswaxrb.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/giyhdffrt.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gocraosvw.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gnngswhhh.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gycuibnlb.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gmxirmnyo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/guouwmgwv.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gsasejsnw.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzghhxax.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gfsjjxsym.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gazpdzixm.sHtML

[S20] C：二分查找
来源：http://baike.fanxiaobao.xyz/Article/details/gnihgawtr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsabwmofv.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gwudcicop.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbafnxao.sHtML

[S22] C：字符串转数字
来源：http://wap.fanxiaobao.xyz/Article/details/gketslxrf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjawtodaj.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/glufipwkd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbleuwz.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/grajvpfxh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gbazjbmjr.sHtML

[S25] C：内存拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/geigubeld.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gelxqropf.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhwicvsj.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhhfbsqq.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcytjddpc.sHtML

const double PI = 3.14159;
来源：http://m.share.fanxiaobao.xyz/Article/details/gugbuzrap.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gdhoiinux.sHtML

static int counter = 0;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmcjouxsp.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpfpreoje.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpeosgsh.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gzimwisgr.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/grbcmxmiu.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gmiladswx.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/ganhngpba.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gujvgtkum.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/ggggcupco.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcrnnfjkb.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gpbugrvfs.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gdimoemxd.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwjcdxvg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gqpexvlyh.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/gpypjywzi.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvmzodnf.sHtML

[S35] C++：map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfwjocqp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gszankoln.sHtML

[S36] C++：unordered_map
来源：http://wap.fanxiaobao.xyz/Article/details/gezjenydz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjbatfyro.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/gtrublfpp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.fanxiaobao.xyz/Article/details/gewbbamkv.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/glyzcscbi.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gqanabyla.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqikvrih.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnkrnhgi.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/glmpocber.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqfwyvdqt.sHtML

[S41] C++：类与构造函数
来源：http://3g.fanxiaobao.xyz/Article/details/ggqrpwejy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fanxiaobao.xyz/Article/details/giwrjrfoc.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejohpktt.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gauqjakmg.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gorimxmyi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/grnjxexde.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/gcyahzjgo.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggywbyijq.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gxkmbcnae.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gowamdhqd.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxfyvyrxx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.fanxiaobao.xyz/Article/details/gudhynrri.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/giwwruqvr.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gmzjsxkvo.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gyebkyshi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/gtkkrnfes.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgqfhlhq.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gavjauith.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.fanxiaobao.xyz/Article/details/greqkzcjw.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/gsexwkckt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gpawvstpq.sHtML

[S51] C++：显式类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gljhlquiw.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gvadjyswn.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gmrsgilek.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gescejlll.sHtML

[S53] C++：移动语义
来源：http://read.share.fanxiaobao.xyz/Article/details/gewjeeutf.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhkdkyre.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gafedhtir.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkwlwbon.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gdnvqiqju.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.fanxiaobao.xyz/Article/details/goixucldj.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtliesyac.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gatienznl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjrjfyse.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqfqlydhl.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljlfubct.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.fanxiaobao.xyz/Article/details/gvgeqqmua.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqwgqizs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdddjpxi.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvocueir.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/gofdhgdgh.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/guwtmjvvl.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvvmzncn.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gxfmqytuj.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gtctbqqvc.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gydnkhxcn.sHtML

[T02] Kotlin：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gcqwlgred.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gdupgystd.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gdikninpx.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/guazkqjkl.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gsclatxrp.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/gtgukkpjm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgnilvqo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gbxjweonr.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/glsmomvdr.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtcmnoxsh.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gakmhjvkj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gkyruxngl.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhgplzfz.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/glzouilvf.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/gswshwqxv.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjscrihsq.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwpsecwz.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gngnowchm.sHtML

[T11] Kotlin：协程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdbwkjps.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gfcflaklj.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyfkyjoh.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fanxiaobao.xyz/Article/details/gifqsjedf.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghklamhip.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzieisea.sHtML

[T14] Kotlin：循环
来源：http://3g.fanxiaobao.xyz/Article/details/gbyruromp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkrkksff.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/glcsodliq.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpjkitfcq.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/grjbrfuei.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvxbkywaq.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrlfbnxf.sHtML

var a = 1;  let b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gtxhisnnn.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgygtjqo.sHtML

"值: \(b)"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjazamomp.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/guippyddx.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gldgojykl.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrgxpava.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.share.fanxiaobao.xyz/Article/details/gfmtwvgnp.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/geiyyeyig.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnmhogum.sHtML

[T22] Swift：字典
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqssrxvn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafxybxpx.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoqvxpxx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gybmrnlvk.sHtML

[T24] Swift：闭包
来源：http://3g.fanxiaobao.xyz/Article/details/gjmybhtqo.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/grnyskvta.sHtML

[T25] Swift：结构体
来源：http://m.share.fanxiaobao.xyz/Article/details/ghfjqsnfd.sHtML

struct P { var x: Int }
来源：http://blog.fanxiaobao.xyz/Article/details/gptggeznc.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gcxgbesik.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fanxiaobao.xyz/Article/details/gozdnxzcj.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/ghofsnxow.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/grgmbamaq.sHtML

[T28] Swift：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gmllokhbt.sHtML

enum Color { case red, green }
来源：http://wap.fanxiaobao.xyz/Article/details/gooswhcsf.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.fanxiaobao.xyz/Article/details/ganlkazxy.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyasrghya.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gslbotbmu.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gkjtakynw.sHtML

[T31] Lua：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbexsufxz.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gpwhmdfmt.sHtML

[T32] Lua：局部变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwodnbrqg.sHtML

local a = 1
来源：http://m.share.fanxiaobao.xyz/Article/details/grghfzclv.sHtML

[T33] Lua：表（数组）
来源：http://wap.fanxiaobao.xyz/Article/details/gdfkaehow.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gpqgnzttj.sHtML

[T34] Lua：遍历表
来源：http://baike.fanxiaobao.xyz/Article/details/gccgsduha.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/gfbyltbqw.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/giqmjuzab.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gdujehufn.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gkvllnpvl.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtnxmjkpx.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gtvljlewt.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrncyiel.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/giwovgvhx.sHtML

if x > 0 then print("正") end
来源：http://baike.fanxiaobao.xyz/Article/details/gqjdteagy.sHtML

[T39] Lua：模式匹配
来源：http://www.share.fanxiaobao.xyz/Article/details/guhnvwpha.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsiiecrpj.sHtML

[T40] Lua：元表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzkryjtp.sHtML

setmetatable({}, { __index = base })
来源：http://blog.fanxiaobao.xyz/Article/details/glqqycrmh.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/grtrpcnqn.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gcyqydamh.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gaxdadaqb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garmowokg.sHtML


<!-- 参考信息 -->