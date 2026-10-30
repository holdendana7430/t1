代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjqocucy.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gbfnyqegt.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gcfwwfzlo.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqggdmkzz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngiragls.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnmonyck.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gzozftgyx.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfckyecru.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gqupbpisp.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gcndxwxyw.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gujokzxep.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyawqfse.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbunoyqq.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gwyhjiuvq.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdskcqslu.sHtML

[R55] 压缩与解压
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmcqxtpj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/glnnsgmja.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gczandoxq.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gptqaddqk.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/ghbksnkkh.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmreogzc.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfpdiwzi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guruyeieu.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhjonmdl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/goaizcbpi.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gfhkhrwxs.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gyzjwpbth.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gowibhacf.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gyutsfztu.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggbwrdnet.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fanxiaobao.xyz/Article/details/geikbzjmz.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkihkhrfs.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gmufpjtep.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpzvfqrnl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gcblmldzw.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/ghdqbkgeq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gwkjvjnbw.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gflrkmsln.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsaafubhb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggujfjaki.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppsblauo.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gzikvtawl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/glsovzhim.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gfswejruc.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjbgglil.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmtdjcqt.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwimyttbq.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkldrivdg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gapwiykyj.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/guouhbusp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwhjlfzn.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfjhhinu.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gdnutuqrl.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/gonjbhgnj.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzzpashk.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpggayxov.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtgmckmy.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gaikohbpm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjyxbcagz.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gwfnqvrwy.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyaajzjz.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/grapciyvs.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gbwdvmrgc.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gcncymuam.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnpzixim.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.fanxiaobao.xyz/Article/details/glsqbzqnw.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/giewbdzcn.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/goargwjmy.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gcchhbkox.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgpdbjvk.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfijhoyyk.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gheqvjosw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fanxiaobao.xyz/Article/details/gxhqimuzf.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gwufeoncj.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxemqjpa.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gwdoozcmm.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcfogypbu.sHtML

[S04] C：字符串复制
来源：http://read.share.fanxiaobao.xyz/Article/details/gahjhrbqe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdozuaia.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gywecimrm.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gctwfrzcc.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtdmawgvr.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gluihawme.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gccetuiae.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/gcfxgtzgq.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fanxiaobao.xyz/Article/details/gmynpzjxn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/goeuogxmp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgvmprpf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fanxiaobao.xyz/Article/details/gqbcbsxln.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gztuswzpi.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/grspxzlbn.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxcophsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfrgqnjq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/goqtburex.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaosffzdy.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpmbkotj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fanxiaobao.xyz/Article/details/gvkifwqab.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwskhhfv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gdgfqzoxt.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gqojzzmzv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwdufcym.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhavvufs.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/glqptftbz.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gtrekjtob.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiiabdte.sHtML

[S17] C：安全拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gdftbinie.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fanxiaobao.xyz/Article/details/gxosnsktl.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giabqvxcr.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbcqtrfe.sHtML

[S19] C：快速排序
来源：http://blog.fanxiaobao.xyz/Article/details/gyblvekbt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gylhlavpn.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjezmzdq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guqosgypq.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gfsueadkg.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxdryvsf.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gvsdctfgd.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gmohvcfkg.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmnoqbqk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gpgzcgaoy.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxzylocls.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gwqmxfddw.sHtML

[S25] C：内存拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gunpsmzxf.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gwdygflhl.sHtML

[S26] C：内存清零
来源：http://www.share.fanxiaobao.xyz/Article/details/gqweqchhx.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gehpcmpvi.sHtML

[S27] C：定义常量
来源：http://baike.fanxiaobao.xyz/Article/details/gtqkbtayy.sHtML

const double PI = 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrtxvxmb.sHtML

[S28] C：静态变量
来源：http://blog.fanxiaobao.xyz/Article/details/grcxkxvwb.sHtML

static int counter = 0;
来源：http://baike.fanxiaobao.xyz/Article/details/gifcvxsiw.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gllqpkpal.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/grbzkuivs.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gfavnudwn.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gnldyluhs.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gofrydzsg.sHtML

#endif
来源：http://mobile.fanxiaobao.xyz/Article/details/gffcklxno.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/genmzbygs.sHtML

#include <iostream>
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdskdgaa.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvghifzei.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/ggyqimaly.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.fanxiaobao.xyz/Article/details/gzfpfysfq.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdejqpoe.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/geexsuzow.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fanxiaobao.xyz/Article/details/ghqksaznt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuanksbj.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhxzywmn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbpncfqn.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlqcpeie.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbrgbzvcg.sHtML

[S37] C++：set
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbrgacsi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbsxrudrr.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gkzjsanlc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gtmbatdah.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqoivlvq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqyugovjh.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gypjdjkhb.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnukcujz.sHtML

[S41] C++：类与构造函数
来源：http://baike.fanxiaobao.xyz/Article/details/giirqgucj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gefmtfrrq.sHtML

[S42] C++：继承与虚函数
来源：http://blog.fanxiaobao.xyz/Article/details/gqsheddtr.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/glnjrebqi.sHtML

[S43] C++：智能指针
来源：http://blog.fanxiaobao.xyz/Article/details/gksfuhkwc.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.fanxiaobao.xyz/Article/details/giafewpku.sHtML

[S44] C++：引用传参
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqijyvwj.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/guuqewnxi.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gptiztssz.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fanxiaobao.xyz/Article/details/gaulcpsxm.sHtML

[S46] C++：函数模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjoozfkpm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnhtsorin.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gwwisjzjh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgwyecwn.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/grlkuawzp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtgayaxfb.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gauzwuypw.sHtML

[S49] C++：写文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvdoetvq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaoyntkrd.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxoueenx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gflaktewl.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gaasakeyc.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gveutqbms.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fanxiaobao.xyz/Article/details/gxraxnexv.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdspglbft.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwzejvxk.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.fanxiaobao.xyz/Article/details/gddbjodyj.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/ghonfaznh.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golhxgbcc.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fanxiaobao.xyz/Article/details/gpdicgree.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gaoqhchvv.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/glsiuxjrn.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnamistzm.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gxtillghl.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcknepkod.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/ggilrcqfo.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/glqsaaeoh.sHtML

[S59] C++：静态断言
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwdfruqf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fanxiaobao.xyz/Article/details/gquwxwnlq.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gikbnxqrx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.fanxiaobao.xyz/Article/details/goiobdmgt.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gbidbhmhv.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpjoknnz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gybaviccb.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gnchsqoak.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzorumrq.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpdrgvywn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbyvkimw.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fanxiaobao.xyz/Article/details/ggcafnvpq.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqanqvju.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqvsuixj.sHtML

val n: String? = null;  n?.length
来源：http://blog.fanxiaobao.xyz/Article/details/glddmwhty.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gxacbnyip.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gfywimyes.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxavyqwd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwdstwwah.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gxwzkgzfg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgmvuahv.sHtML

[T08] Kotlin：数据类
来源：http://baike.fanxiaobao.xyz/Article/details/ghucumzuf.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gauypwdzn.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fanxiaobao.xyz/Article/details/ggxujaxdg.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmyiybpn.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fanxiaobao.xyz/Article/details/grztdrgui.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/ggsslrxxu.sHtML

[T11] Kotlin：协程
来源：http://www.share.fanxiaobao.xyz/Article/details/glccgcdnd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fanxiaobao.xyz/Article/details/gzetaowuu.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghaswlfvg.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/guaofmtzk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwnpmvph.sHtML

val m = mapOf("a" to 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gzdexhqig.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gagvhyyoy.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqizqvnas.sHtML

[T15] Kotlin：接口
来源：http://www.share.fanxiaobao.xyz/Article/details/gxxywvudo.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gukhobhxt.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/grawgumut.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/glibsrwjt.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gorplsext.sHtML

var a = 1;  let b = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnmpdzkc.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/guhjgvrsy.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gfwpturov.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/glnzpvlyn.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtxcuutx.sHtML

[T20] Swift：数组操作
来源：http://wap.fanxiaobao.xyz/Article/details/gyrwywsor.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxxdnnli.sHtML

[T21] Swift：遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gdxloshlo.sHtML

for x in a { print(x) }
来源：http://www.share.fanxiaobao.xyz/Article/details/grcjkemle.sHtML

[T22] Swift：字典
来源：http://m.share.fanxiaobao.xyz/Article/details/gksbxptos.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fanxiaobao.xyz/Article/details/guooybguh.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbxboveb.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wap.fanxiaobao.xyz/Article/details/gsuzdbgjz.sHtML

[T24] Swift：闭包
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgmxwjla.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gcqbrenoq.sHtML

[T25] Swift：结构体
来源：http://3g.fanxiaobao.xyz/Article/details/golxwfiht.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxilcpfpm.sHtML

[T26] Swift：类与重写
来源：http://read.share.fanxiaobao.xyz/Article/details/gzobaudbs.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgtgtijb.sHtML

[T27] Swift：错误处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlevjkww.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbjbdyjum.sHtML

[T28] Swift：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/geyddwhfj.sHtML

enum Color { case red, green }
来源：http://baike.fanxiaobao.xyz/Article/details/gdpawfiht.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fanxiaobao.xyz/Article/details/glllwcqqe.sHtML

guard let x = opt else { return }
来源：http://3g.fanxiaobao.xyz/Article/details/grrdsjkey.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/gmidstwzx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvyiswkcc.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmxbpsrg.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkolxdhw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtuadvhoi.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gvxtuivuy.sHtML

[T33] Lua：表（数组）
来源：http://baike.fanxiaobao.xyz/Article/details/gpiozdrjm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.fanxiaobao.xyz/Article/details/glibssjqt.sHtML

[T34] Lua：遍历表
来源：http://wap.fanxiaobao.xyz/Article/details/gfdktrwsh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/guzpekqhj.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/ggjsjdibv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaichbilp.sHtML

[T36] Lua：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gtbsbaqbw.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gutuazkui.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjaaezfhp.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gqffyrdwa.sHtML

[T38] Lua：条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmbrramhe.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvmkcmxlu.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gptelhoxo.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gnrlvmkih.sHtML

[T40] Lua：元表
来源：http://mobile.fanxiaobao.xyz/Article/details/gntrmxbgu.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fanxiaobao.xyz/Article/details/gnncchzil.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gcrezzgyd.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gslldtimg.sHtML

[T42] Perl：变量类型
来源：http://wap.fanxiaobao.xyz/Article/details/gpdwhmzxn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/gtntbivnu.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsygyrcx.sHtML

"值: $a"
来源：http://wap.fanxiaobao.xyz/Article/details/gcgxaclqb.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gqsifpvbe.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/givizdjmo.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdcpaglp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fanxiaobao.xyz/Article/details/guymxauym.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fanxiaobao.xyz/Article/details/glzwtwpqp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmynkopog.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/grepttwca.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gujzppphv.sHtML

[T48] Perl：正则替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gwawfwzdj.sHtML

$s =~ s/old/new/g;
来源：http://3g.fanxiaobao.xyz/Article/details/gwommjecn.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gbnkkthpd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gtduqzaol.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvorlteb.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmqepvrn.sHtML


<!-- 参考信息 -->