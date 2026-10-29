代发 wailian999

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gmgktpzbs.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/ggbqvivoc.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gotbwtfyl.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gjhwgicka.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gfgxlptwq.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/gzntlzqix.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gfbbgalqd.sHtML

[R43] 按名字查找文件
来源：http://3g.fehbvm.com/Article/details/gtachiiep.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/guiwthauy.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gnlwnpkzf.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gyonybyxu.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/ghzyjchow.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gecnjfpch.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gytadnxwk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gxlieoafp.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gdjlfhzqu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gntvkanrf.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gmtxpftja.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gafmpzcqy.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gglatkxzb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.zdbjq.cn/Article/details/gclfnrewd.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/gcoziccdr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gzvyoqdjc.sHtML

[R51] 排序去重取前几
来源：http://read.share.fehbvm.com/Article/details/gjtxndcjc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gxbigbaoq.sHtML

[R52] 统计行数
来源：http://mobile.hesvh.cn/Article/details/gyxyivwid.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/gratiejfu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gpswfmppu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/ghydfkmup.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gglxicvrl.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gkxvaeeaa.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gszfxazbk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gywkpqrhk.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/guujxbtss.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gwaucthaa.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gmhcpyrkf.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gujabadbm.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gpufzbpzl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/ghzyzxpfk.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gytsevaby.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gfvcuaslu.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gyzzjhoyn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gkbnokcmi.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gdpabifqs.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gwwfumfjc.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gstagdyva.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gzhslsuld.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gffzkdxwv.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gqlfvkcvw.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gnfzfgzmo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fehbvm.com/Article/details/gsdpqvmux.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/ghqgrphyo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gwbnjsgct.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gkibzisjq.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gokypztco.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gvakanqnm.sHtML

openssl rand -hex 16
来源：http://3g.fehbvm.com/Article/details/gapmuibex.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/ggijxbtpk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/ggsfpnpxe.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gesjnlsbc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gmkrppded.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gwatvtfot.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gloipsync.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gekkexlzv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gtqzxatvk.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gjjwfjpvh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gzefwcvtg.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gjyilebhq.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gonvqkpal.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gvsqlhcnc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fehbvm.com/Article/details/gnjmnzdhy.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/gnvjwmdam.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.zdbjq.cn/Article/details/gbayfvnwy.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gsclavxbs.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gsiskatrr.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gyevdhskn.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gffxanjgj.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gpvuqykyv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/gudhfyjgm.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gqxemusqx.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/glavhispj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.hesvh.cn/Article/details/guwbouhrz.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/giyhdyvyx.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gseqzwscm.sHtML

S. C / C++ 专题
来源：http://www.share.fehbvm.com/Article/details/gjasdmdnu.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gyahhtzhq.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gjgypqjjy.sHtML

#include <stdio.h>
来源：http://mobile.zdbjq.cn/Article/details/grpstcnsb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.fehbvm.com/Article/details/gekzzneic.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gclnphdso.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fehbvm.com/Article/details/gmilgqomv.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gptoxcenq.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/ghxszazku.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gevaeltpl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gskuqpmxf.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/guyiojgrt.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gxyhdiviz.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/goptbnjrs.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/giysxmati.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gyfppdjhy.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.hesvh.cn/Article/details/gqrhbezio.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gabwzrqhu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/gkpzxetvy.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gvhtbuptx.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.zdbjq.cn/Article/details/gilbrzxhi.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/ggkpovmao.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gcnrlpgpz.sHtML

[S11] C：逐行读文件
来源：http://blog.fehbvm.com/Article/details/gwfmcvlvw.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/gfvvszqdh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gxoyzhwkw.sHtML

fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gbdiksdww.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ggefbccym.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fehbvm.com/Article/details/gwuykrzei.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/guvcyokth.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.hesvh.cn/Article/details/gxcfqaoax.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gbhgrmnlb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gjcvhoonw.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gdexjqibe.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gyyvnydkg.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/grtffvfvl.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gdwviejdd.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gwuiryhiw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gnwyesfno.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gmwwxoowh.sHtML

int main(int argc, char **argv)
来源：http://blog.fehbvm.com/Article/details/gatqvomhz.sHtML

[S19] C：快速排序
来源：http://baike.hesvh.cn/Article/details/gbnnqegrf.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gftoorzue.sHtML

[S20] C：二分查找
来源：http://m.share.hesvh.cn/Article/details/golvzjlly.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gpylluyiz.sHtML

[S21] C：字符类别判断
来源：http://baike.zdbjq.cn/Article/details/gfcfsdybc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/ggdmopfrd.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gjdaujuid.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gsqrxuuvx.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gjwrzgizk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gdwrmmdqw.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/gopjsilux.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gwhukppdw.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gtpuxsdpl.sHtML

memcpy(dst, src, n);
来源：http://wap.fehbvm.com/Article/details/gkkojstll.sHtML

[S26] C：内存清零
来源：http://www.m.share.hesvh.cn/Article/details/gywwiorco.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gyesvkoyl.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gktxzqlhg.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/giuuozgbl.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/grneffoac.sHtML

static int counter = 0;
来源：http://www.share.fehbvm.com/Article/details/gyqoyaosa.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gzxrsyoym.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/ghomgrkfh.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/guxycousj.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/guhbvwqvh.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/ghlmmypxw.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gkvqyqfam.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gazoekzfs.sHtML

#include <iostream>
来源：http://mobile.zdbjq.cn/Article/details/ggmoyxgjw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.zdbjq.cn/Article/details/gnxqbhqoq.sHtML

[S32] C++：字符串
来源：http://m.share.hesvh.cn/Article/details/gsrpjqbjq.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.zdbjq.cn/Article/details/gxygxnekp.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gxfqxuddf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gltlvcdfi.sHtML

[S34] C++：遍历 vector
来源：http://mobile.hesvh.cn/Article/details/gycctgkpo.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/glqhbzioc.sHtML

[S35] C++：map
来源：http://wap.fehbvm.com/Article/details/gxvsatdmq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gilduwsgw.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.zdbjq.cn/Article/details/ghmiupubm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/glchssxjf.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gflsnqblc.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gaqpozknn.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/gkuinhruk.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.zdbjq.cn/Article/details/gnurkblge.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gvbyhtmqf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.zdbjq.cn/Article/details/gieyhwiec.sHtML

[S40] C++：查找元素
来源：http://baike.hesvh.cn/Article/details/gmuetgcgy.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.fehbvm.com/Article/details/gsvndnfcf.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/gbxpwksja.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/grbyopyjv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/geeropyiq.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gnyzorqpw.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gdneusxip.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fehbvm.com/Article/details/gbjwqwgbr.sHtML

[S44] C++：引用传参
来源：http://wap.hesvh.cn/Article/details/glqmbgyvc.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gcaczdpps.sHtML

[S45] C++：lambda
来源：http://read.share.zdbjq.cn/Article/details/gnahfbpcr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gprdxfisp.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gmfixywtb.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://3g.hesvh.cn/Article/details/gompqnvkq.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.hesvh.cn/Article/details/gjyylztlf.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gwuxaqzbv.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gglcjxyat.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/gwnxytijy.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gyjqnonaz.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/gunbmyqvz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gkiapenpi.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gunucbfhd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/ggepaskjm.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gmmsxxcye.sHtML

static_cast<double>(a) / b
来源：http://mobile.hesvh.cn/Article/details/gpizufryg.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.hesvh.cn/Article/details/gjmbndnar.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/gfqukegjl.sHtML

[S53] C++：移动语义
来源：http://blog.zdbjq.cn/Article/details/glyazojbo.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/glqidvwmi.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gpscwzcxe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gliryxnxx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fehbvm.com/Article/details/gccrciqwa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.fehbvm.com/Article/details/gwxsignwd.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gfxxsrzcc.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.fehbvm.com/Article/details/gjjzvrwnx.sHtML

[S57] C++：编译期常量
来源：http://baike.fehbvm.com/Article/details/gdzgtbrmv.sHtML

constexpr int N = 10;
来源：http://blog.hesvh.cn/Article/details/glleecqxh.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gbnulxfio.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gbfjrlhga.sHtML

[S59] C++：静态断言
来源：http://mobile.fehbvm.com/Article/details/grwxjcspe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/gbdxnbzld.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.zdbjq.cn/Article/details/gxhayidfd.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/glsjzycnt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggqjroqdq.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/ghvtrvisx.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gfzwbynbb.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbrwdallf.sHtML

println("Hello")
来源：http://www.share.hesvh.cn/Article/details/ghqtkawvo.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gfetavyjh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gdugadpxn.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gmgxqnjhz.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/gigfrwhez.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.zdbjq.cn/Article/details/gvnrktbuo.sHtML

val n: String? = null;  n?.length
来源：http://baike.fehbvm.com/Article/details/gkjtnfxgc.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.fehbvm.com/Article/details/gzaqslrsr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/ghfiyrjpc.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.zdbjq.cn/Article/details/gpjusttyu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmfvgic.sHtML

[T07] Kotlin：集合过滤
来源：http://3g.fehbvm.com/Article/details/gwhrokrey.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/ggczukbgg.sHtML

[T08] Kotlin：数据类
来源：http://baike.zdbjq.cn/Article/details/ghvkiliwi.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gmsimaetz.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.hesvh.cn/Article/details/gqtbwiwre.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/guhkvdexf.sHtML

[T10] Kotlin：默认参数
来源：http://3g.fehbvm.com/Article/details/gskhjmevx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/gfsokzudx.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gdmuqpczo.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fehbvm.com/Article/details/gizqbqdfl.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gldfcvubk.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.fehbvm.com/Article/details/goruyfmlb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/ghzgdxikk.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gxpuwrutz.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gsbghdodg.sHtML

for (i in 1..10) println(i)
来源：http://read.share.hesvh.cn/Article/details/gsoqripdr.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/gibjvqaqx.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gvkxdgxml.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gsccimzmi.sHtML

print("Hello")
来源：http://wap.hesvh.cn/Article/details/gtdmlspzj.sHtML

[T17] Swift：变量与常量
来源：http://m.share.hesvh.cn/Article/details/gysilypzl.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gzeiprddl.sHtML

[T18] Swift：字符串插值
来源：http://wap.zdbjq.cn/Article/details/gcosibcpa.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gmjxnipjq.sHtML

[T19] Swift：可选绑定
来源：http://baike.fehbvm.com/Article/details/gfrsayngw.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/getluznrh.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gpihpqady.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/gcqajcanf.sHtML

[T21] Swift：遍历
来源：http://www.blog.hesvh.cn/Article/details/gwviyoyig.sHtML

for x in a { print(x) }
来源：http://www.m.share.fehbvm.com/Article/details/gepqftoid.sHtML

[T22] Swift：字典
来源：http://m.share.hesvh.cn/Article/details/gcuujoghv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gzoqsjoga.sHtML

[T23] Swift：函数
来源：http://wap.hesvh.cn/Article/details/gysaexhqs.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.fehbvm.com/Article/details/gevcslgkf.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gudcxgqtq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.zdbjq.cn/Article/details/grzcxmolk.sHtML

[T25] Swift：结构体
来源：http://mobile.fehbvm.com/Article/details/grnslfkzj.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gyhkxvrin.sHtML

[T26] Swift：类与重写
来源：http://wap.zdbjq.cn/Article/details/gqhhfssyq.sHtML

class A: Base { override func f() {} }
来源：http://m.share.fehbvm.com/Article/details/gteiqhlzi.sHtML

[T27] Swift：错误处理
来源：http://3g.zdbjq.cn/Article/details/grhsclktw.sHtML

do { try f() } catch { print(error) }
来源：http://wap.hesvh.cn/Article/details/gtfsbpfri.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gujkdzjrn.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/glazicrws.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gdovzfhgo.sHtML

guard let x = opt else { return }
来源：http://mobile.fehbvm.com/Article/details/gwumzlitn.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/gjlmdbxco.sHtML

protocol Shape { func area() -> Double }
来源：http://blog.fehbvm.com/Article/details/gozjjmpks.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/giadzjlqb.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gtrxuicoi.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gubowrsci.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gbgkhagaa.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.hesvh.cn/Article/details/gsbqmitaq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fehbvm.com/Article/details/gbfvhsqty.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gwdgcofhd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/guaomngnt.sHtML

[T35] Lua：字典表
来源：http://blog.zdbjq.cn/Article/details/guiymxwrx.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gpbvfisrm.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gvesqdeqw.sHtML

function add(a, b) return a + b end
来源：http://read.share.hesvh.cn/Article/details/ghtihafbb.sHtML

[T37] Lua：字符串拼接
来源：http://3g.hesvh.cn/Article/details/gtustwfun.sHtML

"a" .. "b"
来源：http://www.m.share.hesvh.cn/Article/details/gxivwcujv.sHtML

[T38] Lua：条件
来源：http://wap.hesvh.cn/Article/details/ghlrhkltq.sHtML

if x > 0 then print("正") end
来源：http://mobile.hesvh.cn/Article/details/ghimqlrkt.sHtML

[T39] Lua：模式匹配
来源：http://baike.zdbjq.cn/Article/details/gaayyytlf.sHtML

string.find(s, "%d+")
来源：http://3g.fehbvm.com/Article/details/gigvelpfh.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gtogcxrrg.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.zdbjq.cn/Article/details/gvvpvqvmj.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gatwxzojc.sHtML

print "Hello\n";
来源：http://baike.zdbjq.cn/Article/details/gbqxgqqex.sHtML

[T42] Perl：变量类型
来源：http://3g.zdbjq.cn/Article/details/gtsubinhh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.fehbvm.com/Article/details/gdeylwbjd.sHtML


<!-- 参考信息 -->