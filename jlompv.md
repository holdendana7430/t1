代发 wailian999

cmd > out.log 2>&1
来源：http://hz.yvedp.cn/gthwxerygh.html

[R40] 追加写日志
来源：http://hz.shanyushiyangkeji.top/gtzqnrknzu.html

echo "log" >> out.log
来源：http://hz.0kj1m.cn/gtwaleneji.html

[R41] 丢弃输出
来源：http://hz.daxiang520.top/gtaojgttwb.html

cmd >/dev/null 2>&1
来源：http://hz.jyoumei.cn/gtculjmbgl.html

[R42] 输入重定向
来源：http://hz.fzhhl.top/gtcegmjxag.html

wc -l < a.txt
来源：http://hz.snrcjt.cn/gtuirqyalp.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtmifrbtya.html

find . -name "*.log" -type f
来源：http://hz.yj20258.top/gtcroslekn.html

[R44] 按修改时间查找
来源：http://hz.svipenyu.cn/gtlpuwxtkk.html

find . -mtime -7 -type f
来源：http://hz.c1oappe.top/gtenvlwchh.html

[R45] 批量删除
来源：http://hz.316326.xyz/gtkyzzbfty.html

find . -name "*.tmp" -delete
来源：http://hz.fzhhl.top/gtebnjkbao.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtdlsnvcer.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hfpthk.cn/gtspctrdbj.html

[R47] sed 单行替换
来源：http://hz.yanxiufei.cn/gthjcvpdfp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xingfuxueyuan.xyz/gtuhbfqckx.html

[R48] awk 取指定列
来源：http://hz.yueranfly.top/gtyixtpuot.html

awk '{print $1, $3}' a.txt
来源：http://hz.316326.xyz/gtdavolarl.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gtjohunxqm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.kuanghao11.cn/gtsritwlny.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gttdhlaozf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gogol.net.cn/gtdesbgadb.html

[R51] 排序去重取前几
来源：http://hz.cdnleiting.top/gtoldzchwu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtxzgpblsn.html

[R52] 统计行数
来源：http://hz.yanxiufei.cn/gtgpktibzu.html

wc -l a.txt
来源：http://hz.hysaishi.cn/gtlyxubyoj.html

[R53] 查看文件头与实时尾
来源：http://hz.iojbl.cn/gtpfnzwzjr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gtiyjjpxnt.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtymsgybob.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtrnxcaynb.html

[R55] 压缩与解压
来源：http://hz.yongpay.top/gtvyuaptlt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.birdmap.top/gtopucvbzy.html

[R56] 远程拷贝
来源：http://hz.yuanzhike.top/gtklkteqbi.html

scp file user@host:/path/
来源：http://hz.bjfxy.top/gtsqfxddyw.html

[R57] 远程执行命令
来源：http://hz.shanyushiyangkeji.top/gtecpqpncm.html

ssh user@host 'uptime'
来源：http://hz.sxryk.cn/gtcranhgzy.html

[R58] 下载文件
来源：http://hz.yj20258888.top/gtpwwkxwvs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cheryme.top/gtwlbyevaa.html

[R59] 发 POST JSON
来源：http://hz.yanxiufei.cn/gtkwsslbdu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj202588.top/gtjsjdivxz.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhaomingkeji.xyz/gtzpzgekgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.smart0.xyz/gtpouwldwi.html

[R61] 磁盘占用
来源：http://hz.bjfxy.top/gtsblclzgi.html

df -h;  du -sh *
来源：http://hz.hammf.cn/gthvaqlrgd.html

[R62] 找最占空间的文件
来源：http://hz.xuetiantiany.cn/gthxcnlqca.html

du -ah . | sort -rh | head -10
来源：http://hz.nwbrower.top/gtlcjkyqso.html

[R63] 内存与进程
来源：http://hz.gzhubu.top/gtlozpwbbz.html

free -h;  ps aux | grep nginx
来源：http://hz.birdmap.top/gtqqcekgpv.html

[R64] 结束进程
来源：http://hz.shanyushiyangtech.top/gtmdqwzrbk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.redwolf501.top/gtmbmprdzc.html

[R65] 查看端口占用
来源：http://hz.shuidangran.top/gtovybcfkp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cqqwz.cn/gtrkeqycfd.html

[R66] 定时任务
来源：http://hz.bjfxy.top/gtgalmxiau.html

crontab -e;  crontab -l
来源：http://hz.ydjk.org.cn/gtxmvbldry.html

[R67] 生成随机十六进制串
来源：http://hz.cheryme.top/gtjnmrhkcr.html

openssl rand -hex 16
来源：http://hz.redwolf501.top/gttsvzunqf.html

[R68] 计算文件校验值
来源：http://hz.yj202588.top/gtzcbhpdar.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.c1oappe.top/gtknumfixj.html

[R69] 生成随机密码
来源：http://hz.sxryk.cn/gtcrgxegar.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydzc1.top/gttlougwsk.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtnxczjdym.html

date +%s;  date -d @1700000000
来源：http://hz.cucudq.cn/gtebgclpqd.html

[R71] 日期格式化
来源：http://hz.hnqzz.top/gtswtedzve.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xylfe.cn/gtgrhjhdcz.html

[R72] 等待端口就绪
来源：http://hz.hnqzz.top/gtgwykwawu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtijqvqlhb.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtpqdnmptd.html

split -l 1000 big.log part_
来源：http://hz.chenlongwang.top/gtxecntmfv.html

[R74] 批量重命名
来源：http://hz.yuxming.cn/gtnkwhxted.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xylfe.cn/gtygrxvpyu.html

[R75] 导出环境变量
来源：http://hz.xuetiantiany.cn/gtygtyiaov.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xuetiantiany.cn/gtxuosqgdx.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtoatsbdip.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dashuyun.cn/gtwwhuwsls.html

[R77] 读取用户输入
来源：http://hz.hysaishi.cn/gtzlhfqask.html

read -rp "请输入: " ans
来源：http://hz.xuetiantiany.cn/gteqwfhoaf.html

[R78] 交互式菜单
来源：http://hz.gogol.net.cn/gtpnzsddmk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhiwuduotai.top/gtgyatvtko.html

[R79] 解析命令行选项
来源：http://hz.shuidangran.top/gtbzxiptbs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jianghu66.top/gtoffogkjw.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtfrvkmfab.html

time ./run.sh
来源：http://hz.hfpthk.cn/gtwtlirhal.html

================================================================================
来源：http://hz.havefunace.top/gtmyyfrqqw.html

S. C / C++ 专题
来源：http://hz.nanxuanxn.top/gtiuqnlnzi.html

================================================================================
来源：http://hz.zhixingplan.top/gtdwyhfujc.html

[S01] C：Hello World
来源：http://hz.ppjwa.cn/gtwgkwzvzp.html

#include <stdio.h>
来源：http://hz.xinyue.icu/gthehqqiku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daxiang520.top/gtfoyqcohs.html

[S02] C：变量与格式化输出
来源：http://hz.ivvv.top/gtutmnweoo.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtewqindbx.html

[S03] C：读入整数
来源：http://hz.jianghu66.top/gtrwevkoji.html

int x; scanf("%d", &x);
来源：http://hz.xziqi.cn/gtaplhlzft.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gtwykzlvpd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtotnrvjyw.html

[S05] C：字符串长度
来源：http://hz.daxiang520.top/gtcxumwamf.html

strlen(s)
来源：http://hz.ybcxt.top/gtdmakujyr.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gtvsbyqugs.html

strcmp(a, b) == 0
来源：http://hz.xuetiantiany.cn/gtvyqiijhb.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtddniwsiq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gtqvqznudy.html

[S08] C：动态内存分配与释放
来源：http://hz.nanxuanxn.top/gtsbzrurct.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhijiandao.cn/gtfufeflbw.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigufen.top/gthjturfwz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ivvv.top/gtwoapixyv.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtdsnbyxfy.html

int *p = &a;  *p = 5;
来源：http://hz.cqqwz.cn/gtehrjjbyv.html

[S11] C：逐行读文件
来源：http://hz.jinghuilouyu.cn/gtzqnkyanh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtkbnrobtu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.52xcode.cn/gtymynkiua.html

fclose(f);
来源：http://hz.hysaishi.cn/gtrdqwixac.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gtnystnnov.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fzhhl.top/gtmwsfpwcp.html

[S13] C：宏定义
来源：http://hz.fengsongda.top/gtslktkrlw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xziqi.cn/gtbcfavqmg.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtnwknjswd.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yuxming.cn/gtzxieqccr.html

[S15] C：类型转换
来源：http://hz.nanxinkj.top/gtawdacgep.html

(double) a / b
来源：http://hz.ivvv.top/gtevxioyht.html

[S16] C：位操作置位
来源：http://hz.zhoulong.xyz/gtlojzdiqo.html

x |= (1 << 3);
来源：http://hz.jlsjyb.cn/gtfpnbdrbz.html

[S17] C：安全拼接字符串
来源：http://hz.havefunace.top/gteolnnpwm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shuidangran.top/gtmactipqp.html

[S18] C：命令行参数
来源：http://hz.xziqi.cn/gtgwwqvdbc.html

int main(int argc, char **argv)
来源：http://hz.ehwqpu.com/gtiyraqgty.html

[S19] C：快速排序
来源：http://hz.jlsjyb.cn/gtopovzxia.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtwunyrqte.html

[S20] C：二分查找
来源：http://hz.tianlin.xyz/gtrmwqcxem.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hongshengwenyu.top/gtkpqwladd.html

[S21] C：字符类别判断
来源：http://hz.ybcxt.top/gtlgdtnrvn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtmdfmhtih.html

[S22] C：字符串转数字
来源：http://hz.yangfankeji.com/gtectvrfgg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuetiantiany.cn/gtifncygby.html

[S23] C：随机数
来源：http://hz.cheryme.top/gtqhcbqxsl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.redwolf501.top/gtlshqndnb.html

[S24] C：获取本地时间
来源：http://hz.yonumen.top/gtqbzpqilk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yueranfly.top/gtdvcvmubp.html

[S25] C：内存拷贝
来源：http://hz.daria6918.cn/gtaxbomsor.html

memcpy(dst, src, n);
来源：http://hz.snrcjt.cn/gtexdcxtwx.html

[S26] C：内存清零
来源：http://hz.xuetiantiany.cn/gtcepochhf.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtgsinjtnk.html

[S27] C：定义常量
来源：http://hz.meibo888.top/gtwferwnam.html

const double PI = 3.14159;
来源：http://hz.snrcjt.cn/gtypdzpcxl.html

[S28] C：静态变量
来源：http://hz.yvedp.cn/gtmgwyvtut.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtslglahfa.html

[S29] C：变参函数
来源：http://hz.jqgufenzy.top/gtrtslnxsy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj20258888.top/gthqvcpyrw.html

[S30] C：头文件保护
来源：http://hz.tianlin.xyz/gttygevuxp.html

#ifndef X_H
来源：http://hz.shanyushiyangtech.top/gtybysdkfb.html

#define X_H
来源：http://hz.smart0.xyz/gtpmthwcvs.html

#endif
来源：http://hz.pycfn.com/gtfwdatgtk.html

[S31] C++：Hello World
来源：http://hz.fzhhl.top/gtomniipce.html

#include <iostream>
来源：http://hz.andypj.xyz/gtdhekorbm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.guowangkeji.top/gtmkqldmnt.html

[S32] C++：字符串
来源：http://hz.birdmap.top/gtmohkeblu.html

std::string s = "hi";  s += "!";
来源：http://hz.c1oappe.top/gthmyukoel.html

[S33] C++：vector 增删
来源：http://hz.zycfv.cn/gtbtgrheau.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtmbnvidvh.html

[S34] C++：遍历 vector
来源：http://hz.ybcxt.top/gtzlwgplis.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.fengsongda.top/gtracxnwjm.html

[S35] C++：map
来源：http://hz.yvedp.cn/gtudyshiio.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtzavmdwis.html

[S36] C++：unordered_map
来源：http://hz.sysykeji.top/gtvywprygk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtewiwzofu.html

[S37] C++：set
来源：http://hz.cdnleiting.top/gtkemrautr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangtech.top/gtralqgyvi.html

[S38] C++：排序
来源：http://hz.ivvv.top/gtdfypikyi.html

std::sort(v.begin(), v.end());
来源：http://hz.shzxlz.cn/gttometaph.html

[S39] C++：自定义比较器排序
来源：http://hz.yuanzhike.top/gtzoowtqno.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yanxiufei.cn/gtjcjfwlqv.html

[S40] C++：查找元素
来源：http://hz.guowangkeji.top/gtogxotrwu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.gaohongyu789.top/gtqikkviae.html

[S41] C++：类与构造函数
来源：http://hz.zhiwuduotai.top/gtihphuipv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hfpthk.cn/gtantczbtj.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gthkwdnzxx.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuanzhike.top/gtqvcvdmas.html

[S43] C++：智能指针
来源：http://hz.birdmap.top/gtlbbcbgyl.html

auto p = std::make_unique<int>(5);
来源：http://hz.tianlin.xyz/gtzzhuppsd.html

[S44] C++：引用传参
来源：http://hz.iojbl.cn/gttveohpmr.html

void inc(int &x) { ++x; }
来源：http://hz.andypj.xyz/gtrszxwtjc.html

[S45] C++：lambda
来源：http://hz.quarkkingdee.top/gtxisxemeu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhengqikj.top/gtywiomkyq.html

[S46] C++：函数模板
来源：http://hz.zhengqikj.top/gtwiurtlms.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fzhhl.top/gtabkzwxbq.html

[S47] C++：结构化绑定遍历
来源：http://hz.cqqwz.cn/gthecxxfgg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.nanxuanxn.top/gtvlpgnoco.html

[S48] C++：逐行读文件
来源：http://hz.yuxming.cn/gtnxotmnyr.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.redwolf501.top/gtsqbpsqov.html

while (std::getline(in, line)) { }
来源：http://hz.316326.xyz/gtyzvjikbp.html

[S49] C++：写文件
来源：http://hz.haohaochexian.top/gtxlvfjfvy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtdszrdkyh.html

[S50] C++：格式化数字
来源：http://hz.jinqigufen.top/gtkzwvjnii.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.vqdsnc.cn/gtzjuorggb.html

[S51] C++：显式类型转换
来源：http://hz.jqgfzy.top/gtmfjnukrs.html

static_cast<double>(a) / b
来源：http://hz.zhongyouzk.top/gtiuesexgf.html

[S52] C++：const 与 noexcept
来源：http://hz.bjfxy.top/gtlqpavdzr.html

int size() const noexcept { return n_; }
来源：http://hz.zhiwuduotai.top/gttopnektg.html

[S53] C++：移动语义
来源：http://hz.jqgufenzy.top/gtpqhsxmlv.html

std::vector<int> w = std::move(v);
来源：http://hz.chenzaomai.com/gtcmgggoiu.html

[S54] C++：异常处理
来源：http://hz.hywenlv.cn/gttifeukne.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.xingfuxueyuan.xyz/gtqyptqpfx.html

[S55] C++：结构化绑定
来源：http://hz.chenjidiqi.icu/gtskfxkjta.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yanxiufei.cn/gtbmeeahmd.html

[S56] C++：optional
来源：http://hz.xylfe.cn/gtudbpcdke.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenlongwang.top/gtdrkjsgcj.html

[S57] C++：编译期常量
来源：http://hz.zhaomingkeji.xyz/gtcjturakk.html

constexpr int N = 10;
来源：http://hz.xuetiantiany.cn/gtqnpthfay.html

[S58] C++：命名空间
来源：http://hz.yueranfly.top/gtjfinnihm.html

namespace ns { int f() { return 1; } }
来源：http://hz.nanxuanxn.top/gtohurfugw.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtfidfiobo.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pycfn.com/gtrdspifzr.html

[S60] C++：遍历并删除元素
来源：http://hz.shanyushiyangkeji.top/gtbdvggtje.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtqlyuwfbx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtkzfnlcbo.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnxiangtu.top/gtgztxyohd.html

================================================================================
来源：http://hz.ybcxt.top/gtorcjusjo.html

[T01] Kotlin：Hello World
来源：http://hz.zhongyouzk.top/gtakqgedkl.html

println("Hello")
来源：http://hz.snrcjt.cn/gtxhqnkyub.html

[T02] Kotlin：变量
来源：http://hz.xuanzx.com/gtpmcqkruq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hfpthk.cn/gtjxdbdbhx.html

[T03] Kotlin：字符串模板
来源：http://hz.yongpay.top/gtxtfnhfcx.html

"值: $b"
来源：http://hz.nwbrower.top/gtoqzugdrk.html

[T04] Kotlin：空安全
来源：http://hz.jyoumei.cn/gtuotcysuu.html

val n: String? = null;  n?.length
来源：http://hz.fzhhl.top/gtmymtjaht.html

[T05] Kotlin：when 表达式
来源：http://hz.fengsongda.top/gttiwqzvvt.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cdnleiting.top/gtuekcypdm.html

[T06] Kotlin：集合映射
来源：http://hz.snrcjt.cn/gtdwfleswd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.bjfxy.top/gtuxfwpxuq.html

[T07] Kotlin：集合过滤
来源：http://hz.zhijiandao.cn/gtscfdlpgq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jinqigufen.top/gtthftgaei.html

[T08] Kotlin：数据类
来源：http://hz.jinyuanbaomall.cn/gtdkmxvmlf.html

data class User(val name: String, val age: Int)
来源：http://hz.ydjk.org.cn/gtvktuupky.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gtkfpmdxtn.html

fun String.exclaim() = this + "!"
来源：http://hz.yuxming.cn/gtngfbiulv.html

[T10] Kotlin：默认参数
来源：http://hz.jinyuanbaomall.cn/gtjtgieogs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sysykeji.top/gtzpnvhpxp.html

[T11] Kotlin：协程
来源：http://hz.sysykeji.top/gthobchvpo.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinqigfzy.top/gthffcopvp.html

[T12] Kotlin：解构声明
来源：http://hz.jianghu66.top/gtxgdljyll.html

val (a, b) = Pair(1, 2)
来源：http://hz.cdnleiting.top/gtijcenfag.html

[T13] Kotlin：只读 Map
来源：http://hz.zycfv.cn/gtnmsoeazx.html

val m = mapOf("a" to 1)
来源：http://hz.ydzc1.top/gtsyfbinlt.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtcqzhjsui.html

for (i in 1..10) println(i)
来源：http://hz.tianlin.xyz/gtxxnijgqd.html

[T15] Kotlin：接口
来源：http://hz.cashguo.top/gtrxfqqkhd.html

interface Shape { fun area(): Double }
来源：http://hz.zdqjudy.top/gtirhcufon.html

[T16] Swift：Hello World
来源：http://hz.cqqwz.cn/gtzzsrmxvy.html

print("Hello")
来源：http://hz.zhongyouzk.top/gtmpbjyobu.html

[T17] Swift：变量与常量
来源：http://hz.bjfxy.top/gtplhsjkbu.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gtopatytwb.html

[T18] Swift：字符串插值
来源：http://hz.redwolf501.top/gtqmxeuxzj.html

"值: \(b)"
来源：http://hz.xylfe.cn/gtfvandxzi.html

[T19] Swift：可选绑定
来源：http://hz.yj202588.top/gttvmobuba.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtlhlaunfm.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gtpasaqhuk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gtcvsbmpjk.html

[T21] Swift：遍历
来源：http://hz.hongshengwenyu.top/gtsjesoknw.html

for x in a { print(x) }
来源：http://hz.cashguo.top/gtffszmfic.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtqxkewkho.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.nanxinkj.top/gtnwlkkglp.html

[T23] Swift：函数
来源：http://hz.jinqigfzy.top/gtwvhseqes.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jqgufenzy.top/gtxmzrvcwc.html

[T24] Swift：闭包
来源：http://hz.hfpthk.cn/gtjzyrimsw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jyoumei.cn/gtrpwoprxw.html

[T25] Swift：结构体
来源：http://hz.redwolf501.top/gtziwficpx.html

struct P { var x: Int }
来源：http://hz.jiagoushi.top/gtpnwzfmug.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtiihmclyb.html

class A: Base { override func f() {} }
来源：http://hz.hysaishi.cn/gtwbvkojmq.html

[T27] Swift：错误处理
来源：http://hz.fzhhl.top/gtjvcrbhca.html

do { try f() } catch { print(error) }
来源：http://hz.zhongyouzk.top/gtsimubrxj.html

[T28] Swift：枚举
来源：http://hz.ppjwa.cn/gtbgjosttl.html

enum Color { case red, green }
来源：http://hz.xinyue.icu/gtyesgamlp.html

[T29] Swift：guard 提前返回
来源：http://hz.shangyingyoupin.top/gthlckwazw.html

guard let x = opt else { return }
来源：http://hz.zhijiandao.cn/gtqxrbyooi.html

[T30] Swift：协议
来源：http://hz.smart0.xyz/gtixblmelh.html

protocol Shape { func area() -> Double }
来源：http://hz.jqgufenzy.top/gtsjouotit.html

[T31] Lua：Hello World
来源：http://hz.sxryk.cn/gtynjsaqds.html

print("Hello")
来源：http://hz.iojbl.cn/gtlehilqsr.html

[T32] Lua：局部变量
来源：http://hz.pengpengdd.cyou/gtrjfpbrtw.html

local a = 1
来源：http://hz.havefunace.top/gtfbmfzscl.html

[T33] Lua：表（数组）
来源：http://hz.andypj.xyz/gtejpfybtl.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.meibo888.top/gtsplhknrn.html

[T34] Lua：遍历表
来源：http://hz.0kj1m.cn/gtsmnusylm.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.jqgfzy.top/gtndipeikg.html

[T35] Lua：字典表
来源：http://hz.jqgfzy.top/gtpequapmw.html

local d = { a = 1 };  d.b = 2
来源：http://hz.yuxming.cn/gtsrkpwwbb.html

[T36] Lua：函数
来源：http://hz.hammf.cn/gtmlthzeaj.html

function add(a, b) return a + b end
来源：http://hz.ehwqpu.com/gtlzsciwmm.html

[T37] Lua：字符串拼接
来源：http://hz.aibaodan.cn/gtvqkxvoux.html

"a" .. "b"
来源：http://hz.zdqjudy.top/gtledbeaqw.html

[T38] Lua：条件
来源：http://hz.yanxiufei.cn/gtzcnvqkmn.html

if x > 0 then print("正") end
来源：http://hz.cashguo.top/gtxemvnkrl.html

[T39] Lua：模式匹配
来源：http://hz.svipenyu.cn/gtnjproglk.html

string.find(s, "%d+")
来源：http://hz.zhiwuduotai.top/gtjpwjkxsg.html

[T40] Lua：元表
来源：http://hz.gogol.net.cn/gtnzrfyhtm.html

setmetatable({}, { __index = base })
来源：http://hz.yj20258888.top/gtpkzjubjf.html

[T41] Perl：Hello World
来源：http://hz.yueranfly.top/gtnadsheec.html

print "Hello\n";
来源：http://hz.yuanzhike.top/gtccuspyhr.html

[T42] Perl：变量类型
来源：http://hz.zhaomingkeji.xyz/gtrprncede.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.chenjidiqi.icu/gtxipqqnqr.html


<!-- 参考信息 -->