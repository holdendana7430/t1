代发 wailian999

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/grirafnlg.sHtML

[R44] 按修改时间查找
来源：http://m.share.hesvh.cn/Article/details/gbetdbgqr.sHtML

find . -mtime -7 -type f
来源：http://mobile.zdbjq.cn/Article/details/gbegyzdqy.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/gqbpojycr.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gbitlknqz.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gquqasiuf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/giddjrtui.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/gcxbrogok.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/grdmfuord.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/gicaijnsx.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gaszmjjod.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gszurfhwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gtapyjrnm.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gjvejvynp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmmmrjgyt.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gkkqvgqbr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gdhhtovvw.sHtML

[R52] 统计行数
来源：http://3g.fehbvm.com/Article/details/gbahfthoo.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gzjucsttn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gykcvgime.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gveqflkhb.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gvdhqkgdo.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/goohzexob.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gvangchub.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/grlwvdgvj.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gkrwwsixp.sHtML

scp file user@host:/path/
来源：http://www.m.share.hesvh.cn/Article/details/gzzqsaldm.sHtML

[R57] 远程执行命令
来源：http://read.share.hesvh.cn/Article/details/gnjacqioe.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gsexmnyqo.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gefdiwvva.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gxejebujd.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gbasewmvc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gquxusgrb.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gmsjhbuoi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/ggcjgaxmt.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gaxqnsohc.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gtrnhyron.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gbpongbkc.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gjcuxtanb.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/greqmkkal.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gmigqfnfw.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gzsnreoay.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gasjmelvf.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gqoiwagyq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/ggmjbbnjm.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gewfayahw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gctwjyhnu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gpaoaguxo.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gvlkirqnq.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/ghzlazcuf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/glnhbcrqv.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gsgdhxzzx.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fehbvm.com/Article/details/gklaguqlt.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gvtdxdqlb.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gnqgedbcf.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/glxkisnsk.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gancypyxt.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/gxqaazoro.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gthouuxok.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/grcemgpas.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/gbmcsqxdj.sHtML

[R74] 批量重命名
来源：http://baike.fehbvm.com/Article/details/gqfspelve.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gjbgizurd.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gcgdnujjf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gtddsyric.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gxnlndnui.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gwyrqagzl.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gwnprsaeb.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gongffdaz.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gqvfoickz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.zdbjq.cn/Article/details/grzglappx.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gonyptlag.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/glwckielc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/giynzghtu.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gisguyklh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gljdfgdhl.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gthqteuuf.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gzrxcgziv.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/grtoqlqgk.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gsktysrgv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://wap.fehbvm.com/Article/details/gfbyjksbr.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.hesvh.cn/Article/details/gigsbvhix.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gkpuuksdb.sHtML

[S03] C：读入整数
来源：http://www.share.hesvh.cn/Article/details/gulzliyoi.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gzlfafbbo.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/guwtqxdun.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/gxfqnvqtr.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gtskgbvfp.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/gksrmnqer.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gsavckorl.sHtML

strcmp(a, b) == 0
来源：http://wap.zdbjq.cn/Article/details/glnshjupn.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/govgaxmqt.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gzffdntvg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.zdbjq.cn/Article/details/ghudaivzw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.zdbjq.cn/Article/details/ggpvndtbb.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/geqgwilnn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.fehbvm.com/Article/details/gtlxhadkh.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gdjkrsrnk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gsuiqvmmc.sHtML

[S11] C：逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gmgssxkrr.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gbyzmazmi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.zdbjq.cn/Article/details/gqosgvsac.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gbcyklfqc.sHtML

[S12] C：写文件
来源：http://read.share.fehbvm.com/Article/details/gmyvpwppm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gravkszwe.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gmdoutvgs.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gynpaepau.sHtML

[S14] C：枚举
来源：http://www.share.hesvh.cn/Article/details/gvkywmlhi.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gmfuophbr.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gzwnxobri.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/gluszlknv.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gmnebxlqz.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/ghvkodrxn.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/geheaotzr.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.hesvh.cn/Article/details/gyigkeopk.sHtML

[S18] C：命令行参数
来源：http://read.share.hesvh.cn/Article/details/gmajxtjvd.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gcqqjowqc.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/gfjsyvwuk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gkptjnncs.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/gksphekvl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gpqkcgyri.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gnrdsvwfn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fehbvm.com/Article/details/giepqvegc.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gvrjtmkfc.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gejzoonlm.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gcyaphvdj.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/grvulhsdu.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/guwjjjhan.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gaqzaezkw.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gtksriggd.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/gatwiiuhy.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gvnkowrok.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/geeizqkka.sHtML

[S27] C：定义常量
来源：http://wap.zdbjq.cn/Article/details/ggcktewhb.sHtML

const double PI = 3.14159;
来源：http://blog.fehbvm.com/Article/details/gdtpsbcbm.sHtML

[S28] C：静态变量
来源：http://www.share.fehbvm.com/Article/details/gcwzxqnyv.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/grydzgrmd.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/getskicnp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.zdbjq.cn/Article/details/gvrdeuufg.sHtML

[S30] C：头文件保护
来源：http://3g.zdbjq.cn/Article/details/gudisbhui.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/gaaflhvgm.sHtML

#define X_H
来源：http://www.share.fehbvm.com/Article/details/gqerthbms.sHtML

#endif
来源：http://mobile.fehbvm.com/Article/details/gncqrunfp.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/grizndzsg.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gxqaqvfol.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gbkdogvbt.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gihjisqbh.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.hesvh.cn/Article/details/gnkpokwah.sHtML

[S33] C++：vector 增删
来源：http://wap.hesvh.cn/Article/details/gttmcbefb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.hesvh.cn/Article/details/gurhjicnw.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fehbvm.com/Article/details/goapnnvij.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gcyugipus.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gcagetbta.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gkgfymmap.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gntvcibgj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/ghzvtczsq.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/gqqtwhmkt.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/ghqsdkzph.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gnnergkwo.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gogzurfsy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fehbvm.com/Article/details/ghfsqnopm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.zdbjq.cn/Article/details/grtlsryeh.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gvvzzzyjn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gllenkfgr.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gzllrsage.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gifqaaskw.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gsdmkbwmz.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/ghwtmwtcw.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gisoomaxp.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gbdltimbo.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/glreblxct.sHtML

void inc(int &x) { ++x; }
来源：http://3g.hesvh.cn/Article/details/gbbeuywbg.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/glblvhyko.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ggverthgo.sHtML

[S46] C++：函数模板
来源：http://m.share.hesvh.cn/Article/details/gdilwqpsd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.zdbjq.cn/Article/details/gnvivrvyd.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gwzzcgbuq.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/giavhvjxp.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gtridgzsy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fehbvm.com/Article/details/gvvsiqljy.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gnanbroul.sHtML

[S49] C++：写文件
来源：http://wap.hesvh.cn/Article/details/goqzpgwui.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gdxgjqyxv.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gxfpaflln.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.hesvh.cn/Article/details/gxbkrtqun.sHtML

[S51] C++：显式类型转换
来源：http://read.share.zdbjq.cn/Article/details/geljkrudx.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/goarytybo.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/gtrwbnklz.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gndhlgvzn.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/ggsksidao.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gqivhhsxs.sHtML

[S54] C++：异常处理
来源：http://read.share.fehbvm.com/Article/details/gbjefxrmr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fehbvm.com/Article/details/gpzhvchgv.sHtML

[S55] C++：结构化绑定
来源：http://baike.zdbjq.cn/Article/details/gjnyaoepv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fehbvm.com/Article/details/gylxyhxjf.sHtML

[S56] C++：optional
来源：http://wap.fehbvm.com/Article/details/gqifydbzj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fehbvm.com/Article/details/glmlvpodz.sHtML

[S57] C++：编译期常量
来源：http://wap.fehbvm.com/Article/details/gzlxsryky.sHtML

constexpr int N = 10;
来源：http://wap.fehbvm.com/Article/details/gggbtxnfo.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gqhtkvxri.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gbgjpeuuv.sHtML

[S59] C++：静态断言
来源：http://mobile.hesvh.cn/Article/details/gdacsxzlj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fehbvm.com/Article/details/gebentgkk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gftqtpfqa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gvtrcclie.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gvsbubitb.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/geowjaclc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gzdztultm.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbbkqdsdd.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gxsdphafq.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gnklhxwoe.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.zdbjq.cn/Article/details/gefwdgqww.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gdrqfjjqv.sHtML

"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gmmtgupoc.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gxbnqfxha.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gvykhubmy.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.fehbvm.com/Article/details/gipklwxaa.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gyrijpcpi.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gwhqnknlx.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmgvnbsyd.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.fehbvm.com/Article/details/ggfmjwstn.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.zdbjq.cn/Article/details/gdaualesi.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gzvlvqfqe.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.zdbjq.cn/Article/details/gudndnycp.sHtML

[T09] Kotlin：扩展函数
来源：http://wap.fehbvm.com/Article/details/gwjynhhqh.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gbjwwtdlb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gupdoimsc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.hesvh.cn/Article/details/geckrvzgt.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gonfzervu.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fehbvm.com/Article/details/gtlnteugh.sHtML

[T12] Kotlin：解构声明
来源：http://wap.hesvh.cn/Article/details/ggtzesoqi.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.zdbjq.cn/Article/details/gcwyuisvo.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.fehbvm.com/Article/details/gqajxjsep.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gymwxpcjb.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.hesvh.cn/Article/details/gorzktiro.sHtML

for (i in 1..10) println(i)
来源：http://3g.hesvh.cn/Article/details/gajuiewsk.sHtML

[T15] Kotlin：接口
来源：http://m.share.hesvh.cn/Article/details/gjqagdlnb.sHtML

interface Shape { fun area(): Double }
来源：http://baike.hesvh.cn/Article/details/gpxcxmpfd.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/ghzsifosf.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gldxgvjcq.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/gqathlgaq.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gledcyjmi.sHtML

[T18] Swift：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gmmtchkrv.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/gtmljjvnt.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gxynqciuc.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gqavpcafp.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.zdbjq.cn/Article/details/gidfjfsfi.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gwofgqajg.sHtML

[T21] Swift：遍历
来源：http://3g.fehbvm.com/Article/details/gocdfiheo.sHtML

for x in a { print(x) }
来源：http://www.blog.zdbjq.cn/Article/details/gtgukpnxx.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gkkrgvmoh.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://baike.hesvh.cn/Article/details/gtprrofqj.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gmvgijchu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gunpijomx.sHtML

[T24] Swift：闭包
来源：http://3g.hesvh.cn/Article/details/goydimscv.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.fehbvm.com/Article/details/gvpptires.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gedgxfkna.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gqpskatqh.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gpupncile.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gicydeupa.sHtML

[T27] Swift：错误处理
来源：http://www.share.zdbjq.cn/Article/details/gfvhkfwal.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gvxxampnx.sHtML

[T28] Swift：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gtmgwawne.sHtML

enum Color { case red, green }
来源：http://3g.fehbvm.com/Article/details/gdtjxiqrc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.zdbjq.cn/Article/details/gimjxjmek.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gjdgjczwn.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gkpvtqwxd.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.hesvh.cn/Article/details/gutvrqriq.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdbjgxjaj.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gffwawnlt.sHtML

[T32] Lua：局部变量
来源：http://m.share.hesvh.cn/Article/details/gpdarhxwt.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/grgrxmqwd.sHtML

[T33] Lua：表（数组）
来源：http://mobile.zdbjq.cn/Article/details/glhmvyers.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gkirjxbfx.sHtML

[T34] Lua：遍历表
来源：http://3g.zdbjq.cn/Article/details/gksachpyt.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.fehbvm.com/Article/details/gihlmiegt.sHtML

[T35] Lua：字典表
来源：http://blog.hesvh.cn/Article/details/gesgjgndt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.zdbjq.cn/Article/details/gbhqfeugx.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gapoiyssf.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gqewjrywc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/goqaorgrn.sHtML

"a" .. "b"
来源：http://baike.zdbjq.cn/Article/details/gjololyon.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gsyfbpoug.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gbtcbkqqj.sHtML

[T39] Lua：模式匹配
来源：http://3g.fehbvm.com/Article/details/gbqlqpnhn.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gmtzlhfxm.sHtML

[T40] Lua：元表
来源：http://www.blog.zdbjq.cn/Article/details/gdaxlkmzm.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.hesvh.cn/Article/details/gqkdeytme.sHtML

[T41] Perl：Hello World
来源：http://wap.fehbvm.com/Article/details/ghndvtcvz.sHtML

print "Hello\n";
来源：http://read.share.zdbjq.cn/Article/details/glfitbxmy.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gfcrlpmdn.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fehbvm.com/Article/details/gsdqqxbjy.sHtML

[T43] Perl：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gxgdukrer.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/gozvbyzfn.sHtML

[T44] Perl：条件
来源：http://www.blog.zdbjq.cn/Article/details/gezxqgmet.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/gbyfcwaqo.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gvwodzdcn.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/glmitcdzl.sHtML

[T46] Perl：哈希操作
来源：http://read.share.fehbvm.com/Article/details/gqvbcgpdz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gglimcqyl.sHtML


<!-- 参考信息 -->