代发 wailian999

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gnyulvpqm.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gydjwhjqo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gixxucigv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.hesvh.cn/Article/details/gbytlcilr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/guudqtrak.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gbqqkbqzr.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gknlegxlx.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/ggibuxdqu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.hesvh.cn/Article/details/gestdviuz.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gibxxypzf.sHtML

wc -l < a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gcwsyotkp.sHtML

[R43] 按名字查找文件
来源：http://3g.zdbjq.cn/Article/details/geamlwlhd.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fehbvm.com/Article/details/gsfftetma.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gmkzlsjel.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gjkjqwmfj.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gyqmizcnc.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gmiifmyns.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gxvbijlde.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/glhcainyc.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gkzwrlrwa.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/guqswbfjk.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gmnfpnsiw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/grgqxeisj.sHtML

[R49] awk 带条件
来源：http://blog.fehbvm.com/Article/details/gilnlytns.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/glubfhtng.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gncunkpqk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gnigypwzs.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/ggyolqlto.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gjxqwefta.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gqjdiuwrs.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/ggjcgljas.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gmkuihyaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gtutsmrec.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/girkcpnff.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gapneuumm.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/grfqchzdu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gucqxudal.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gwnualxft.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/giluxyovb.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gttchpogz.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gkorrkjqr.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gpoukpokv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gcpchloum.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gxiqwxnjh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/giiqpyqcu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fehbvm.com/Article/details/gbdpagseb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.zdbjq.cn/Article/details/gjhcghfqv.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gawqjefcp.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/galxpfxfr.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gsmtjvcro.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.zdbjq.cn/Article/details/ghhvkhbbh.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gucydgznc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gsflhepre.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gramnqtwf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/geuoiglvf.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gzzsolwmb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gnrgadiir.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gqgctyzwc.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gfioyyyhv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gytqofjue.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gijjcmelb.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gdoxbwema.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/ggiwcbmua.sHtML

[R69] 生成随机密码
来源：http://blog.fehbvm.com/Article/details/gtrxlxays.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gcbsglqse.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/gjkhuuxlu.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gjforvwtd.sHtML

[R71] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/geimoqyyr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gzbsqdguv.sHtML

[R72] 等待端口就绪
来源：http://read.share.hesvh.cn/Article/details/gnitczczp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gzmfsieqt.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/ggaerbpwx.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gctmyguvi.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gxrmjpbns.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gzzrulhtk.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/gzkgoplyc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/gomvxpyvu.sHtML

[R76] 使用临时文件
来源：http://read.share.hesvh.cn/Article/details/gfocgeeee.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gyhlcrtlz.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gckvabuwj.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/guvvkrmgl.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/gmqihwwjh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/ghrgxhvql.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gvbadlphq.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/gdpobabdz.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/guzoohzxb.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gylaximuu.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbplqolkq.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gelybtaty.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gwtasbunr.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghelmrksr.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/ggvcenhlf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.hesvh.cn/Article/details/gbhsjihmu.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gforyssqh.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/gnfoplyio.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gdbcwyjou.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gzcwkdtuh.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gfjdbfgmi.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.hesvh.cn/Article/details/gstplqiuu.sHtML

[S05] C：字符串长度
来源：http://www.share.fehbvm.com/Article/details/gcmipjbwk.sHtML

strlen(s)
来源：http://www.blog.fehbvm.com/Article/details/gxtlsmnzk.sHtML

[S06] C：字符串比较
来源：http://read.share.hesvh.cn/Article/details/gektgivpk.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/ggizosjro.sHtML

[S07] C：数组遍历求和
来源：http://3g.fehbvm.com/Article/details/gqfxyggwl.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.zdbjq.cn/Article/details/gcuvizqqb.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gwqgvetmh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.hesvh.cn/Article/details/gejibrqbj.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fehbvm.com/Article/details/gstohczqm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gukgycqqq.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gilomhwot.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/geevdcbsm.sHtML

[S11] C：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gxufahgpq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gffiyksof.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gjklkbigq.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/grddxarxm.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gmpwwyijc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gnxpgipcu.sHtML

[S13] C：宏定义
来源：http://3g.fehbvm.com/Article/details/gziohzmqm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/ggnutwnmh.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gbyiirvcx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gikxbhmtw.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gjuhcdtzg.sHtML

(double) a / b
来源：http://baike.zdbjq.cn/Article/details/gtfneujww.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/gstxalnpd.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gyanymnhu.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/glzndoieb.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.zdbjq.cn/Article/details/gwtbzbbef.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gesgswnwq.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/gqpjqcwzz.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gdwlsmjgd.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/glaumgqdd.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/grkmaqsfs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gqnphjhpj.sHtML

[S21] C：字符类别判断
来源：http://blog.hesvh.cn/Article/details/ghkueigkw.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.hesvh.cn/Article/details/gqzatgnrh.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gvvlrwbjl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gcbwdsycw.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gkhwzdkgp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fehbvm.com/Article/details/gdglznjwv.sHtML

[S24] C：获取本地时间
来源：http://read.share.zdbjq.cn/Article/details/gawycxypk.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gtexmtbum.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gynvhchfd.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gbehnxcmk.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gffegxaat.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fehbvm.com/Article/details/gonxowpbb.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/giuoixraa.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/gvbbauffp.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gkcahxfiw.sHtML

static int counter = 0;
来源：http://read.share.hesvh.cn/Article/details/ghtivvwsl.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/gnfvwxkbl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.fehbvm.com/Article/details/gjxwaortc.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/geifcagca.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gfyxdkjah.sHtML

#define X_H
来源：http://3g.fehbvm.com/Article/details/gigmelimu.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gsqqodttj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gksyvqevs.sHtML

#include <iostream>
来源：http://wap.hesvh.cn/Article/details/gjccrzxzu.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.hesvh.cn/Article/details/gxrmakrcd.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/grlonkeiv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gygtluecq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gmwyqzxrq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fehbvm.com/Article/details/gbudnjhqx.sHtML

[S34] C++：遍历 vector
来源：http://baike.fehbvm.com/Article/details/gzkbewgat.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gyzsyuejg.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gwelgprsl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/glpttyttt.sHtML

[S36] C++：unordered_map
来源：http://wap.zdbjq.cn/Article/details/gcosgjpgo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gytkjkasq.sHtML

[S37] C++：set
来源：http://m.share.hesvh.cn/Article/details/gxrdsdsrp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://baike.zdbjq.cn/Article/details/gaxvopiws.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/grinbjcnt.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gfzgqchub.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gwsxxazbt.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/glwbpeaxr.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/guockduid.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gvkbanxro.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gyhonizuk.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gxgainwgf.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.hesvh.cn/Article/details/gnuavkzlr.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gtzmtjhcl.sHtML

[S43] C++：智能指针
来源：http://mobile.fehbvm.com/Article/details/gpvesjaws.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/ggyqbehxy.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/gjdocvzcz.sHtML

void inc(int &x) { ++x; }
来源：http://3g.zdbjq.cn/Article/details/ggdhfrejz.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/guhcmkmmy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gujzmddfu.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gusknsqnq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/glcgywzgz.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/gnjyabuex.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fehbvm.com/Article/details/gcrmoxbxk.sHtML

[S48] C++：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gedmhlqbm.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gnqqpilbt.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/gzxmwdoxc.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwvqnueek.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/gjnxxnids.sHtML

[S50] C++：格式化数字
来源：http://www.blog.zdbjq.cn/Article/details/gesbyrkya.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gliafbcld.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/giwurwsii.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/gmiqrvyvr.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.hesvh.cn/Article/details/gdvpuxzdd.sHtML

int size() const noexcept { return n_; }
来源：http://wap.zdbjq.cn/Article/details/gykszxovv.sHtML

[S53] C++：移动语义
来源：http://blog.fehbvm.com/Article/details/gugiyxtuu.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.zdbjq.cn/Article/details/giwigfpcc.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gshwraubq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gdcpaaduf.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/goaydgvcb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.zdbjq.cn/Article/details/gmkwcgour.sHtML

[S56] C++：optional
来源：http://read.share.fehbvm.com/Article/details/gnjbzsbyk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gxbmlzvuo.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gfcfetyow.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/girtjzohj.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gimbatqsg.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gfddnwsfe.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gdaeaioca.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gxsojhazt.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gintgfnai.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.hesvh.cn/Article/details/gvlbzlwoo.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gltixzpzs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fehbvm.com/Article/details/gqdcyxhly.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gwjfrkhgj.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gqhiztjqw.sHtML

println("Hello")
来源：http://wap.hesvh.cn/Article/details/gyoowbqeb.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gweswcysk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gvhbbdysr.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.fehbvm.com/Article/details/gvbmzqlhn.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gqqdghkaw.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gpnpuuntt.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.hesvh.cn/Article/details/gkwvkaebx.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fehbvm.com/Article/details/gfchzsinq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gevdooffn.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gouoybbfo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.zdbjq.cn/Article/details/gkilzdhlu.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/giblaldwc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.zdbjq.cn/Article/details/gwfbsvdbu.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gwayiqych.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.hesvh.cn/Article/details/gvzjfevyt.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.hesvh.cn/Article/details/glatonxiz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.hesvh.cn/Article/details/gytglnejw.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gowawnfak.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.blog.fehbvm.com/Article/details/gniaunnxd.sHtML

[T11] Kotlin：协程
来源：http://3g.hesvh.cn/Article/details/glxhpcpzt.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/grfirrcpx.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gwtqbwxfa.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/gjyrjutnc.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gwjthhmve.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.zdbjq.cn/Article/details/gprfxsqpk.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gqcjpflfe.sHtML

for (i in 1..10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/gcfghgqwc.sHtML

[T15] Kotlin：接口
来源：http://m.share.fehbvm.com/Article/details/gzrmwnkxm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fehbvm.com/Article/details/gdypokzca.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/ggujjxigs.sHtML

print("Hello")
来源：http://m.share.hesvh.cn/Article/details/grbfagwsm.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/ghwcbzygb.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.hesvh.cn/Article/details/grzfkyufu.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gfdaappwl.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gzhohfxpb.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gtmkaprvd.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcttmfvny.sHtML

[T20] Swift：数组操作
来源：http://blog.fehbvm.com/Article/details/ggmvxfgmf.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fehbvm.com/Article/details/gsmvtynfo.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/glstpsjee.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gkiylyzpn.sHtML

[T22] Swift：字典
来源：http://wap.zdbjq.cn/Article/details/guvpiwumt.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/gioxkpbjn.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gqszmisss.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://m.share.fehbvm.com/Article/details/gtuknqxwm.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gcykhnmbs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gbsurdqpu.sHtML

[T25] Swift：结构体
来源：http://www.share.zdbjq.cn/Article/details/gkhqnjpps.sHtML

struct P { var x: Int }
来源：http://baike.zdbjq.cn/Article/details/gbhrxkhep.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gnmwvhygm.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gvbbprypa.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gmvrzbvrp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.hesvh.cn/Article/details/gmoemtrvc.sHtML

[T28] Swift：枚举
来源：http://read.share.zdbjq.cn/Article/details/gpewudbqo.sHtML

enum Color { case red, green }
来源：http://www.m.share.zdbjq.cn/Article/details/gspzyuasm.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.hesvh.cn/Article/details/gnuakzsfz.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gxikegkuo.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gmfzmgzmm.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.fehbvm.com/Article/details/glaudhmig.sHtML

[T31] Lua：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gcijdmtne.sHtML

print("Hello")
来源：http://baike.zdbjq.cn/Article/details/gnseqgeaw.sHtML

[T32] Lua：局部变量
来源：http://www.share.hesvh.cn/Article/details/glhhmjwux.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/geqdcexdm.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/grqbdzwry.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://mobile.hesvh.cn/Article/details/gwwqeedee.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gpbmrmqkz.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gaystqwdb.sHtML

[T35] Lua：字典表
来源：http://read.share.zdbjq.cn/Article/details/gvsyatouz.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gclixzind.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gdikstahp.sHtML

function add(a, b) return a + b end
来源：http://3g.hesvh.cn/Article/details/gjxlkeysh.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gpcimdymr.sHtML

"a" .. "b"
来源：http://mobile.zdbjq.cn/Article/details/gsmrqrsuq.sHtML

[T38] Lua：条件
来源：http://www.blog.hesvh.cn/Article/details/gcivretvq.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gtsfproog.sHtML

[T39] Lua：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gwgcvkhcc.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/glehhlugs.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/ghcihsakq.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gycbzzsyf.sHtML


<!-- 参考信息 -->