代发 wailian999

files=$(ls -1)
来源：http://hz.dianchejie.cn/gtxxgltmny.html

[R38] 管道串联
来源：http://hz.haohaochexian.top/gtlftfyoqz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zdqjudy.top/gtpwcyusjg.html

[R39] 重定向标准输出与错误
来源：http://hz.zhixingplan.top/gtdyxquupw.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtsapfvnsx.html

[R40] 追加写日志
来源：http://hz.gaohongyu789.top/gtvlaekqff.html

echo "log" >> out.log
来源：http://hz.pycfn.com/gtwmxzrjzm.html

[R41] 丢弃输出
来源：http://hz.9152youxi.cn/gtjiighxjg.html

cmd >/dev/null 2>&1
来源：http://hz.pycfn.com/gtiknkiklq.html

[R42] 输入重定向
来源：http://hz.ivvv.top/gtdsxlnbgf.html

wc -l < a.txt
来源：http://hz.chenjidiqi.icu/gtkvhgexgq.html

[R43] 按名字查找文件
来源：http://hz.guowangkeji.top/gtieczhbqn.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtnpsrfafc.html

[R44] 按修改时间查找
来源：http://hz.yonumen.top/gtsydignem.html

find . -mtime -7 -type f
来源：http://hz.gotoacloud.top/gtnygkwhzz.html

[R45] 批量删除
来源：http://hz.zhoulong.xyz/gtukemqagq.html

find . -name "*.tmp" -delete
来源：http://hz.chenzaomai.com/gtfxswsqtr.html

[R46] 递归替换文件内容
来源：http://hz.jlsjyb.cn/gtctuetpyc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtvwnvqcum.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtcoqzresg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shuidangran.top/gtqqavjcwn.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtyqmetfnp.html

awk '{print $1, $3}' a.txt
来源：http://hz.xziqi.cn/gtrvznyfwk.html

[R49] awk 带条件
来源：http://hz.yuanzhike.top/gtxhaezspg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.haohaochexian.top/gtsprffogn.html

[R50] awk 求和
来源：http://hz.daria6918.cn/gttpshnemc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtlbpcggzw.html

[R51] 排序去重取前几
来源：http://hz.xinyue.icu/gtiugxjbif.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.316326.xyz/gtqnwrymsk.html

[R52] 统计行数
来源：http://hz.sxryk.cn/gtupqbvfnv.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtsrpqwhqx.html

[R53] 查看文件头与实时尾
来源：http://hz.zdqjudy.top/gtatybtwuv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.smart0.xyz/gtzyslpcnl.html

[R54] 比较两个文件
来源：http://hz.mhx1999.top/gtjcbjwalk.html

diff a.txt b.txt
来源：http://hz.cdnleiting.top/gtupzdiooh.html

[R55] 压缩与解压
来源：http://hz.cheryme.top/gtjbdilxud.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.vqdsnc.cn/gtanvilfab.html

[R56] 远程拷贝
来源：http://hz.snrcjt.cn/gtfsfdxgaf.html

scp file user@host:/path/
来源：http://hz.sysykeji.top/gtquydbadc.html

[R57] 远程执行命令
来源：http://hz.hysaishi.cn/gtovldujzl.html

ssh user@host 'uptime'
来源：http://hz.chenlongwang.top/gtgpfmnamq.html

[R58] 下载文件
来源：http://hz.c1oappe.top/gtnvtxavxj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhaomingkeji.xyz/gtuovuidkh.html

[R59] 发 POST JSON
来源：http://hz.daxiang520.top/gtxqzekxhk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yj20258.top/gtdgpwdahl.html

[R60] 只看 HTTP 状态码
来源：http://hz.nanxinkj.top/gtttfuueap.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.pengpengdd.cyou/gtutnultrz.html

[R61] 磁盘占用
来源：http://hz.svipenyu.cn/gtewcicpcb.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtvsukeqrs.html

[R62] 找最占空间的文件
来源：http://hz.kuanghao11.cn/gtfvkmphlq.html

du -ah . | sort -rh | head -10
来源：http://hz.hfpthk.cn/gtrtcpnasg.html

[R63] 内存与进程
来源：http://hz.sweek.top/gtupgjhbji.html

free -h;  ps aux | grep nginx
来源：http://hz.ydzc1.top/gtunzttjfk.html

[R64] 结束进程
来源：http://hz.ybcxt.top/gtbfmolamd.html

kill -9 $(pgrep -f app.py)
来源：http://hz.tian-w.cn/gtaqpuaabk.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gttsgyswgg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ybcxt.top/gtyuispcjx.html

[R66] 定时任务
来源：http://hz.hysaishi.cn/gtuvwlvrxo.html

crontab -e;  crontab -l
来源：http://hz.zdqjudy.top/gtgexvimgg.html

[R67] 生成随机十六进制串
来源：http://hz.zhaomingkeji.xyz/gtrgtjvzvq.html

openssl rand -hex 16
来源：http://hz.snrcjt.cn/gtyvwfoigh.html

[R68] 计算文件校验值
来源：http://hz.fzhhl.top/gtbygbxbak.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.316326.xyz/gtezrbvdob.html

[R69] 生成随机密码
来源：http://hz.nanxinkj.top/gtjzvtscsg.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258.top/gtizlaewnn.html

[R70] 时间戳与互转
来源：http://hz.jyoumei.cn/gtcjqsstln.html

date +%s;  date -d @1700000000
来源：http://hz.ybcxt.top/gtvhfsmade.html

[R71] 日期格式化
来源：http://hz.hnqzz.top/gtbacxqggo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gtcjggseco.html

[R72] 等待端口就绪
来源：http://hz.pycfn.com/gtmlunpevw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtfrbwaclr.html

[R73] 分割大日志
来源：http://hz.zhaomingkeji.xyz/gtuzzviduv.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtriosffue.html

[R74] 批量重命名
来源：http://hz.hnqzz.top/gtygnwyxyd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhoulong.xyz/gtsayhzmis.html

[R75] 导出环境变量
来源：http://hz.pengpengdd.cyou/gtmhqugzlg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gteeycrlae.html

[R76] 使用临时文件
来源：http://hz.xuetiantiany.cn/gtefrqhkas.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.redwolf501.top/gtttvetsyy.html

[R77] 读取用户输入
来源：http://hz.zhengqikj.top/gtdyhjsvcz.html

read -rp "请输入: " ans
来源：http://hz.tianlin.xyz/gtymhdabsd.html

[R78] 交互式菜单
来源：http://hz.nanxuanxn.top/gtmwyczmun.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenlongwang.top/gtvcqlxdos.html

[R79] 解析命令行选项
来源：http://hz.havefunace.top/gtmxzkiyjn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.xuetiantiany.cn/gtaflcitow.html

[R80] 查看脚本执行耗时
来源：http://hz.ppjwa.cn/gtjdejcshx.html

time ./run.sh
来源：http://hz.ppjwa.cn/gthtfdtrec.html

================================================================================
来源：http://hz.fengsongda.top/gtscvmydtc.html

S. C / C++ 专题
来源：http://hz.xuetiantiany.cn/gtaubkogrq.html

================================================================================
来源：http://hz.ppjwa.cn/gtmjuqutoh.html

[S01] C：Hello World
来源：http://hz.bjfxy.top/gtwtklsvid.html

#include <stdio.h>
来源：http://hz.shuidangran.top/gtosbntcbf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shanyushiyangtech.top/gtkgzuouds.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtqhmtzjft.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gttqymskvs.html

[S03] C：读入整数
来源：http://hz.ppjwa.cn/gtizrtwisc.html

int x; scanf("%d", &x);
来源：http://hz.pengpengdd.cyou/gtgbdbpbfd.html

[S04] C：字符串复制
来源：http://hz.cashguo.top/gtmzfyggmj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.havefunace.top/gtikauvyiq.html

[S05] C：字符串长度
来源：http://hz.quarkkingdee.top/gtcpnxlwiu.html

strlen(s)
来源：http://hz.feifeiyinyue.top/gtziwkylgl.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gtktvtahpg.html

strcmp(a, b) == 0
来源：http://hz.zhaomingkeji.xyz/gtammiecrp.html

[S07] C：数组遍历求和
来源：http://hz.hongshengwenyu.top/gtexuxbcem.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xylfe.cn/gtgulnhzcb.html

[S08] C：动态内存分配与释放
来源：http://hz.gaohongyu789.top/gtpgspxeti.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hysaishi.cn/gtzpeyhqbe.html

[S09] C：结构体定义与初始化
来源：http://hz.cashguo.top/gtqlxelcbv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hysaishi.cn/gthobzsmkp.html

[S10] C：指针与解引用
来源：http://hz.vqdsnc.cn/gtszdmdsxc.html

int *p = &a;  *p = 5;
来源：http://hz.chenzaomai.com/gtcndqarhq.html

[S11] C：逐行读文件
来源：http://hz.vqdsnc.cn/gtanjturls.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.snrcjt.cn/gtkouhdavd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.0kj1m.cn/gtziipizqj.html

fclose(f);
来源：http://hz.9152youxi.cn/gtcwdkriiw.html

[S12] C：写文件
来源：http://hz.ywan-chungtsiang.top/gtqezvnzao.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhiwuduotai.top/gtrthxufdj.html

[S13] C：宏定义
来源：http://hz.xingfuxueyuan.xyz/gtzadcjnni.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuanzhike.top/gtetmutnkl.html

[S14] C：枚举
来源：http://hz.nanxinkj.top/gtuxqlhyyh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sweek.top/gtdnuoleqk.html

[S15] C：类型转换
来源：http://hz.yonumen.top/gtexkdgesr.html

(double) a / b
来源：http://hz.dianchejie.cn/gtblhfhkbs.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtgvfxuaim.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtbtmtxknq.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtxcnklqqv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sysykeji.top/gtibuadpdv.html

[S18] C：命令行参数
来源：http://hz.shangyingyoupin.top/gtuoxwpnhp.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gtlzkexcuj.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtilhhglly.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cashguo.top/gtgbopgfkg.html

[S20] C：二分查找
来源：http://hz.zhixingplan.top/gtuvwccwzh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ivvv.top/gtjbptmylf.html

[S21] C：字符类别判断
来源：http://hz.yj20258888.top/gtarowjhpc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jyoumei.cn/gtlpeilnmt.html

[S22] C：字符串转数字
来源：http://hz.ehwqpu.com/gtkavdiixp.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangkeji.top/gtmgqfgzpa.html

[S23] C：随机数
来源：http://hz.jlsjyb.cn/gttalvurol.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhoulong.xyz/gtryplpuja.html

[S24] C：获取本地时间
来源：http://hz.iojbl.cn/gtyyzqptam.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.pycfn.com/gthzhfhcjt.html

[S25] C：内存拷贝
来源：http://hz.sweek.top/gtfoxobqmp.html

memcpy(dst, src, n);
来源：http://hz.ivvv.top/gtljfchdzf.html

[S26] C：内存清零
来源：http://hz.andypj.xyz/gtaranbevn.html

memset(a, 0, sizeof a);
来源：http://hz.birdmap.top/gtwrceiamz.html

[S27] C：定义常量
来源：http://hz.52xcode.cn/gtzalsbauk.html

const double PI = 3.14159;
来源：http://hz.iojbl.cn/gtanymlmpx.html

[S28] C：静态变量
来源：http://hz.shuidangran.top/gtockhrktk.html

static int counter = 0;
来源：http://hz.cashguo.top/gthcgeogyh.html

[S29] C：变参函数
来源：http://hz.xuanzx.com/gtdniwiasi.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtoojuxvog.html

[S30] C：头文件保护
来源：http://hz.gzhubu.top/gtbzzhqewd.html

#ifndef X_H
来源：http://hz.hammf.cn/gtgncjycuc.html

#define X_H
来源：http://hz.fengsongda.top/gtpwvdryxt.html

#endif
来源：http://hz.yangfankeji.com/gtkkcicewe.html

[S31] C++：Hello World
来源：http://hz.xuetiantiany.cn/gtogxbdokh.html

#include <iostream>
来源：http://hz.jqgfzy.top/gtvbfbpize.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hysaishi.cn/gthgfxtnkf.html

[S32] C++：字符串
来源：http://hz.yuxming.cn/gtnkfvwtyk.html

std::string s = "hi";  s += "!";
来源：http://hz.xuanzx.com/gtjhrqzlqk.html

[S33] C++：vector 增删
来源：http://hz.xziqi.cn/gthvdsjbca.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtzbrkfsei.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtkbjxcavp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydzc1.top/gtkhmfoqdh.html

[S35] C++：map
来源：http://hz.hnqzz.top/gtqtflgmzu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtnsznfrmw.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtdcgfcfvx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtfxupmojd.html

[S37] C++：set
来源：http://hz.yongpay.top/gtcyalpkxi.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daxiang520.top/gtrbxikbav.html

[S38] C++：排序
来源：http://hz.yonumen.top/gtrspwihco.html

std::sort(v.begin(), v.end());
来源：http://hz.meibo888.top/gtntzhxbcb.html

[S39] C++：自定义比较器排序
来源：http://hz.yj20258888.top/gtflnnbwhf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhoulong.xyz/gtgvykhezy.html

[S40] C++：查找元素
来源：http://hz.daxiang520.top/gtbptcrtxy.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.kuanghao11.cn/gtnfwsxbkn.html

[S41] C++：类与构造函数
来源：http://hz.ehwqpu.com/gtohnhzemj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.mhx1999.top/gtgypkwakk.html

[S42] C++：继承与虚函数
来源：http://hz.yuxming.cn/gtelkjqoic.html

class B : public Base { public: void f() override {} };
来源：http://hz.9152youxi.cn/gtyswuiwlq.html

[S43] C++：智能指针
来源：http://hz.aizwys.cn/gtaijcjbkl.html

auto p = std::make_unique<int>(5);
来源：http://hz.iojbl.cn/gtlwegxgpx.html

[S44] C++：引用传参
来源：http://hz.nanxuanxn.top/gtldphotvc.html

void inc(int &x) { ++x; }
来源：http://hz.ydzc1.top/gtottkqwbr.html

[S45] C++：lambda
来源：http://hz.jinqigufen.top/gtdhziucpd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hfpthk.cn/gtpwruemgs.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gtcdbutjrv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.vqdsnc.cn/gtsdmozdzr.html

[S47] C++：结构化绑定遍历
来源：http://hz.316326.xyz/gtjqyvurmu.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yj202588.top/gtcqlcxqml.html

[S48] C++：逐行读文件
来源：http://hz.xinyue.icu/gtbypngshl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jyoumei.cn/gtbmzsablu.html

while (std::getline(in, line)) { }
来源：http://hz.daxiang520.top/gtaihhfjia.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtpbetovtz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zycfv.cn/gthbnompng.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gtepeokkzr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ehwqpu.com/gtfgbdkhed.html

[S51] C++：显式类型转换
来源：http://hz.daxiang520.top/gtlaqfomlr.html

static_cast<double>(a) / b
来源：http://hz.chenjidiqi.icu/gtwdpdmewc.html

[S52] C++：const 与 noexcept
来源：http://hz.9152youxi.cn/gtiewpeund.html

int size() const noexcept { return n_; }
来源：http://hz.quarkkingdee.top/gtnykfyzqp.html

[S53] C++：移动语义
来源：http://hz.hongshengwenyu.top/gtvqfowiok.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtjqokqhyi.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtdypcaewu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigufen.top/gtusojsfot.html

[S55] C++：结构化绑定
来源：http://hz.hnxiangtu.top/gtwfhpsskp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhijiandao.cn/gtqurccvxp.html

[S56] C++：optional
来源：http://hz.zhixingplan.top/gtcogrktpv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sysykeji.top/gtzypiirie.html

[S57] C++：编译期常量
来源：http://hz.shuidangran.top/gtcwcjxhir.html

constexpr int N = 10;
来源：http://hz.xingfuxueyuan.xyz/gtxukjxxpn.html

[S58] C++：命名空间
来源：http://hz.zycfv.cn/gtmorepyfx.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhixingplan.top/gtlakejlao.html

[S59] C++：静态断言
来源：http://hz.gogol.net.cn/gtrabzynve.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yonumen.top/gtkwtqzslx.html

[S60] C++：遍历并删除元素
来源：http://hz.aizwys.cn/gtlueciwxt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.gaohongyu789.top/gtbnmvjohq.html

================================================================================
来源：http://hz.guannengcc.top/gtbvjcujhn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.haohaochexian.top/gtrdomutec.html

================================================================================
来源：http://hz.9152youxi.cn/gtlulhofbt.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtxgqicfsl.html

println("Hello")
来源：http://hz.nwbrower.top/gtczdaypke.html

[T02] Kotlin：变量
来源：http://hz.cheryme.top/gtcdtgbvhm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.smart0.xyz/gtdeuvfkqs.html

[T03] Kotlin：字符串模板
来源：http://hz.tian-w.cn/gtoanqgfwb.html

"值: $b"
来源：http://hz.jinyuanbaomall.cn/gtrvlulixj.html

[T04] Kotlin：空安全
来源：http://hz.cheryme.top/gtrtinjhwm.html

val n: String? = null;  n?.length
来源：http://hz.jqgufenzy.top/gtgdlfiqzx.html

[T05] Kotlin：when 表达式
来源：http://hz.zhixingplan.top/gtsubqlhto.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gtzviahhnq.html

[T06] Kotlin：集合映射
来源：http://hz.jinghuilouyu.cn/gtayqwxfqp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhoulong.xyz/gtknpvgizv.html

[T07] Kotlin：集合过滤
来源：http://hz.guannengcc.top/gtdxtcajqw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.chenlongwang.top/gtaoqimjyp.html

[T08] Kotlin：数据类
来源：http://hz.pengpengdd.cyou/gtjewelazn.html

data class User(val name: String, val age: Int)
来源：http://hz.ywan-chungtsiang.top/gttwpdflqr.html

[T09] Kotlin：扩展函数
来源：http://hz.zhongyouzk.top/gtzzwnuybq.html

fun String.exclaim() = this + "!"
来源：http://hz.0kj1m.cn/gthmrbbcft.html

[T10] Kotlin：默认参数
来源：http://hz.yanxiufei.cn/gthbqtfhtb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.daxiang520.top/gtjirwfruq.html

[T11] Kotlin：协程
来源：http://hz.nanxinkj.top/gtdbtrzpye.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.52xcode.cn/gtbkbgfrgg.html

[T12] Kotlin：解构声明
来源：http://hz.gotoacloud.top/gtaghfjucg.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtpkktpnmw.html

[T13] Kotlin：只读 Map
来源：http://hz.cqqwz.cn/gtltqxhamc.html

val m = mapOf("a" to 1)
来源：http://hz.jinghuilouyu.cn/gthkudlgyp.html

[T14] Kotlin：循环
来源：http://hz.kuanghao11.cn/gtyvomtzmm.html

for (i in 1..10) println(i)
来源：http://hz.52xcode.cn/gtzikhnfcj.html

[T15] Kotlin：接口
来源：http://hz.birdmap.top/gtthsnjbzm.html

interface Shape { fun area(): Double }
来源：http://hz.jqgufenzy.top/gtufilmbpt.html

[T16] Swift：Hello World
来源：http://hz.xinyue.icu/gtfihmczxc.html

print("Hello")
来源：http://hz.bjfxy.top/gtowjrjoqg.html

[T17] Swift：变量与常量
来源：http://hz.shanyushiyangtech.top/gtcemhiahh.html

var a = 1;  let b = 2
来源：http://hz.smart0.xyz/gtvrsqulpa.html

[T18] Swift：字符串插值
来源：http://hz.zycfv.cn/gtnytxkwwj.html

"值: \(b)"
来源：http://hz.fzhhl.top/gtevuwxjcf.html

[T19] Swift：可选绑定
来源：http://hz.redwolf501.top/gtwbghqbzx.html

if let n = opt { print(n) }
来源：http://hz.dianchejie.cn/gtslnlbmya.html

[T20] Swift：数组操作
来源：http://hz.zhengqikj.top/gtwbkgypzz.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yj20258888.top/gtbwlfqkqy.html

[T21] Swift：遍历
来源：http://hz.jlsjyb.cn/gtjcycgxkf.html

for x in a { print(x) }
来源：http://hz.gotoacloud.top/gtqbcmqnsp.html

[T22] Swift：字典
来源：http://hz.zhiwuduotai.top/gtcdurgzez.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.daria6918.cn/gtfpywxgpy.html

[T23] Swift：函数
来源：http://hz.jiagoushi.top/gtprvjfznr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yvedp.cn/gtbcqfjina.html

[T24] Swift：闭包
来源：http://hz.andypj.xyz/gttdvwzuxf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.daxiang520.top/gtxyiwlgee.html

[T25] Swift：结构体
来源：http://hz.ydjk.org.cn/gtqvmnmgyj.html

struct P { var x: Int }
来源：http://hz.zhoulong.xyz/gtvhydmhfp.html

[T26] Swift：类与重写
来源：http://hz.yuanzhike.top/gtbemprbbg.html

class A: Base { override func f() {} }
来源：http://hz.guowangkeji.top/gtvjvzyhzl.html

[T27] Swift：错误处理
来源：http://hz.xingfuxueyuan.xyz/gtvpnysydb.html

do { try f() } catch { print(error) }
来源：http://hz.gogol.net.cn/gtjgilvwux.html

[T28] Swift：枚举
来源：http://hz.feifeiyinyue.top/gtwvkpciqk.html

enum Color { case red, green }
来源：http://hz.aibaodan.cn/gtdhbxpeum.html

[T29] Swift：guard 提前返回
来源：http://hz.jqgufenzy.top/gtxbkzyjdl.html

guard let x = opt else { return }
来源：http://hz.jinqigfzy.top/gtnrthjtid.html

[T30] Swift：协议
来源：http://hz.xziqi.cn/gtbnrbyjdn.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtmgwbnuln.html

[T31] Lua：Hello World
来源：http://hz.smart0.xyz/gtqvptrhrc.html

print("Hello")
来源：http://hz.xziqi.cn/gtldykegxx.html

[T32] Lua：局部变量
来源：http://hz.wangdashe.top/gtlwffuewe.html

local a = 1
来源：http://hz.tian-w.cn/gtsateontt.html

[T33] Lua：表（数组）
来源：http://hz.aibaodan.cn/gtykysqtxm.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.ppjwa.cn/gtprrzisuz.html

[T34] Lua：遍历表
来源：http://hz.jinghuilouyu.cn/gtdifqyeai.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.snrcjt.cn/gtpqtoxlll.html

[T35] Lua：字典表
来源：http://hz.yuanzhike.top/gtmnjkuigb.html

local d = { a = 1 };  d.b = 2
来源：http://hz.sxryk.cn/gtepeehxhi.html

[T36] Lua：函数
来源：http://hz.fzhhl.top/gtvqfyvtlr.html

function add(a, b) return a + b end
来源：http://hz.ydzc1.top/gtofwxayei.html

[T37] Lua：字符串拼接
来源：http://hz.ydzc1.top/gtkbipwtqw.html

"a" .. "b"
来源：http://hz.xylfe.cn/gtkebtjfjo.html

[T38] Lua：条件
来源：http://hz.havefunace.top/gtaoqomugy.html

if x > 0 then print("正") end
来源：http://hz.dianchejie.cn/gtvxoagslh.html

[T39] Lua：模式匹配
来源：http://hz.ivvv.top/gtzzjtoriu.html

string.find(s, "%d+")
来源：http://hz.ppjwa.cn/gtawolbofq.html

[T40] Lua：元表
来源：http://hz.cucudq.cn/gtvzxszgbu.html

setmetatable({}, { __index = base })
来源：http://hz.gogol.net.cn/gtiggbkxor.html


<!-- 参考信息 -->