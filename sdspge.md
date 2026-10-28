代发 wailian999

cmd > out.log 2>&1
来源：http://hz.gotoacloud.top/gtoogjgerk.html

[R40] 追加写日志
来源：http://hz.jlsjyb.cn/gtuppsixoq.html

echo "log" >> out.log
来源：http://hz.c1oappe.top/gtrspmxtbr.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtbokbggbu.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtloswoqqa.html

[R42] 输入重定向
来源：http://hz.birdmap.top/gtztuyahhc.html

wc -l < a.txt
来源：http://hz.jinqigfzy.top/gtedrdwotz.html

[R43] 按名字查找文件
来源：http://hz.iojbl.cn/gtlgvmqrbv.html

find . -name "*.log" -type f
来源：http://hz.jianghu66.top/gtcqypkhuv.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtfngnoubs.html

find . -mtime -7 -type f
来源：http://hz.hysaishi.cn/gtnwtypxaj.html

[R45] 批量删除
来源：http://hz.cdnleiting.top/gtsirhvdxx.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtwsccwmnn.html

[R46] 递归替换文件内容
来源：http://hz.vqdsnc.cn/gtnyplitcy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.feifeiyinyue.top/gtcnckpvbu.html

[R47] sed 单行替换
来源：http://hz.cdnleiting.top/gtngctjucv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zdqjudy.top/gtmtglllhd.html

[R48] awk 取指定列
来源：http://hz.hongshengwenyu.top/gtliqifmmy.html

awk '{print $1, $3}' a.txt
来源：http://hz.redwolf501.top/gtiwbnzrfr.html

[R49] awk 带条件
来源：http://hz.zhoulong.xyz/gtjqdzvkuq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.andypj.xyz/gtqkbpsmwq.html

[R50] awk 求和
来源：http://hz.bjfxy.top/gtmkqmipqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.mhx1999.top/gtilcfozhl.html

[R51] 排序去重取前几
来源：http://hz.dashuyun.cn/gtzitscmjm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gthsvbvqwt.html

[R52] 统计行数
来源：http://hz.dianchejie.cn/gtqgxpmcyb.html

wc -l a.txt
来源：http://hz.daria6918.cn/gtfwrhvgnm.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgfzy.top/gtikgtgiuw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gotoacloud.top/gtjxtmjkdb.html

[R54] 比较两个文件
来源：http://hz.jinyuanbaomall.cn/gtdjvleihc.html

diff a.txt b.txt
来源：http://hz.shanyushiyangtech.top/gtstkfrftl.html

[R55] 压缩与解压
来源：http://hz.zhaomingkeji.xyz/gtphtznikr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhijiandao.cn/gtaqscxlgk.html

[R56] 远程拷贝
来源：http://hz.zhijiandao.cn/gtbcfwlkej.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtidsakaav.html

[R57] 远程执行命令
来源：http://hz.yuanzhike.top/gtmpusovpc.html

ssh user@host 'uptime'
来源：http://hz.aizwys.cn/gtpeixguqo.html

[R58] 下载文件
来源：http://hz.hongshengwenyu.top/gtuetfupfs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cdnleiting.top/gtmrcpuise.html

[R59] 发 POST JSON
来源：http://hz.yuxming.cn/gtjqnwhrkt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigufen.top/gtfzztdvbl.html

[R60] 只看 HTTP 状态码
来源：http://hz.snrcjt.cn/gtnqozsudl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.hysaishi.cn/gtkmkgyvpt.html

[R61] 磁盘占用
来源：http://hz.jlsjyb.cn/gtyipyvwkf.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtrgmxnttf.html

[R62] 找最占空间的文件
来源：http://hz.zhaomingkeji.xyz/gtisbbcwqq.html

du -ah . | sort -rh | head -10
来源：http://hz.shanyushiyangtech.top/gtsxkncivc.html

[R63] 内存与进程
来源：http://hz.c1oappe.top/gtkqihwveo.html

free -h;  ps aux | grep nginx
来源：http://hz.jiagoushi.top/gtogyxsgzb.html

[R64] 结束进程
来源：http://hz.yvedp.cn/gtrnfazewx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtjohdtlpq.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtdykgkfop.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtkmjedyff.html

[R66] 定时任务
来源：http://hz.ydzc1.top/gtgnatojxh.html

crontab -e;  crontab -l
来源：http://hz.zhiwuduotai.top/gtzoaueulu.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtjnpkbodk.html

openssl rand -hex 16
来源：http://hz.iojbl.cn/gtgogyddaq.html

[R68] 计算文件校验值
来源：http://hz.meibo888.top/gtamnfjwoc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.havefunace.top/gtxoqkfyzm.html

[R69] 生成随机密码
来源：http://hz.yuanzhike.top/gtbmybnbwt.html

head -c 16 /dev/urandom | base64
来源：http://hz.sxryk.cn/gtylrkexkx.html

[R70] 时间戳与互转
来源：http://hz.chenzaomai.com/gtexggkcxg.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtnoikjlos.html

[R71] 日期格式化
来源：http://hz.chenzaomai.com/gtmspgppwc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shuidangran.top/gtsnggaryy.html

[R72] 等待端口就绪
来源：http://hz.chenjidiqi.icu/gtahucsijz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fzhhl.top/gtsiawbsjy.html

[R73] 分割大日志
来源：http://hz.xuetiantiany.cn/gtxsypuytj.html

split -l 1000 big.log part_
来源：http://hz.shanyushiyangkeji.top/gtdguvdcha.html

[R74] 批量重命名
来源：http://hz.chenzaomai.com/gtyikwumem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhengqikj.top/gtlidcxctr.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gtovrojcyt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtvkdjqanu.html

[R76] 使用临时文件
来源：http://hz.ivvv.top/gtnwxmglac.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.tian-w.cn/gtgediqqyr.html

[R77] 读取用户输入
来源：http://hz.yonumen.top/gtkszonokw.html

read -rp "请输入: " ans
来源：http://hz.yanxiufei.cn/gtwumepnzh.html

[R78] 交互式菜单
来源：http://hz.316326.xyz/gtlsxlijsz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.shzxlz.cn/gtdquiwnsk.html

[R79] 解析命令行选项
来源：http://hz.redwolf501.top/gtylhqknfb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jiagoushi.top/gtphakduia.html

[R80] 查看脚本执行耗时
来源：http://hz.ehwqpu.com/gtznhygbwz.html

time ./run.sh
来源：http://hz.jlsjyb.cn/gtgymllpli.html

================================================================================
来源：http://hz.havefunace.top/gtoytipanz.html

S. C / C++ 专题
来源：http://hz.andypj.xyz/gtxtyeoobg.html

================================================================================
来源：http://hz.nanxuanxn.top/gtbyipraln.html

[S01] C：Hello World
来源：http://hz.chenzaomai.com/gtgpzgpjdz.html

#include <stdio.h>
来源：http://hz.yj20258888.top/gtjzzrzrea.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtcmckpehz.html

[S02] C：变量与格式化输出
来源：http://hz.bjfxy.top/gtuukwrqzu.html

int a = 10; printf("%d\n", a);
来源：http://hz.fengsongda.top/gtrlebipqc.html

[S03] C：读入整数
来源：http://hz.yonumen.top/gtfffmzsur.html

int x; scanf("%d", &x);
来源：http://hz.yangfankeji.com/gtzcleaeve.html

[S04] C：字符串复制
来源：http://hz.sysykeji.top/gtottpwlls.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yongpay.top/gtadgecomc.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtpidykvir.html

strlen(s)
来源：http://hz.cheryme.top/gtkkrhrpwx.html

[S06] C：字符串比较
来源：http://hz.nwbrower.top/gtypvtbxxa.html

strcmp(a, b) == 0
来源：http://hz.chenjidiqi.icu/gtuzarmzck.html

[S07] C：数组遍历求和
来源：http://hz.hammf.cn/gtrnxrjlzf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtsbfqwlnx.html

[S08] C：动态内存分配与释放
来源：http://hz.jinyuanbaomall.cn/gthtsfteit.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yonumen.top/gtevvfgbkp.html

[S09] C：结构体定义与初始化
来源：http://hz.jlsjyb.cn/gtmhnulnqc.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.aizwys.cn/gtcpywnykg.html

[S10] C：指针与解引用
来源：http://hz.jinqigfzy.top/gtrseswhrr.html

int *p = &a;  *p = 5;
来源：http://hz.xinyue.icu/gtzmuiwzyx.html

[S11] C：逐行读文件
来源：http://hz.ydjk.org.cn/gtgwokkldw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.xingfuxueyuan.xyz/gtevxhyvct.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ehwqpu.com/gthcvnebio.html

fclose(f);
来源：http://hz.gaohongyu789.top/gtapebdqmx.html

[S12] C：写文件
来源：http://hz.ehwqpu.com/gtzqjcnxdr.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtgbrewvpu.html

[S13] C：宏定义
来源：http://hz.zhoulong.xyz/gtetjjqgfm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.guowangkeji.top/gtqbqhlogf.html

[S14] C：枚举
来源：http://hz.dashuyun.cn/gtabsgtuys.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hnxiangtu.top/gtynbkwpav.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtahrhhnmz.html

(double) a / b
来源：http://hz.ehwqpu.com/gtmmaxltpk.html

[S16] C：位操作置位
来源：http://hz.redwolf501.top/gtokriuucg.html

x |= (1 << 3);
来源：http://hz.cashguo.top/gtvrqsbarc.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtucfqyrak.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sweek.top/gtsicaqlvw.html

[S18] C：命令行参数
来源：http://hz.ivvv.top/gtlikseqam.html

int main(int argc, char **argv)
来源：http://hz.chenlongwang.top/gtksebhjfr.html

[S19] C：快速排序
来源：http://hz.ehwqpu.com/gtphwsdord.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.sxryk.cn/gtlusvdekk.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtnodiarcu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cheryme.top/gtfkchnpai.html

[S21] C：字符类别判断
来源：http://hz.xylfe.cn/gtitbylrve.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtvnamupnr.html

[S22] C：字符串转数字
来源：http://hz.xylfe.cn/gtqdtevtpx.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.kuanghao11.cn/gtpnhmakfj.html

[S23] C：随机数
来源：http://hz.zhiwuduotai.top/gtbnomwemz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shzxlz.cn/gtdontczeg.html

[S24] C：获取本地时间
来源：http://hz.ydzc1.top/gtvcwwbitp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydzc1.top/gtcrhvnvrz.html

[S25] C：内存拷贝
来源：http://hz.ybcxt.top/gtebmrjnpa.html

memcpy(dst, src, n);
来源：http://hz.yuanzhike.top/gtacsaqlxx.html

[S26] C：内存清零
来源：http://hz.haohaochexian.top/gtoykudaum.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtbuqqudtz.html

[S27] C：定义常量
来源：http://hz.pengpengdd.cyou/gtvvcpxjpa.html

const double PI = 3.14159;
来源：http://hz.zhixingplan.top/gtaryxbulh.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtbscbbmqt.html

static int counter = 0;
来源：http://hz.zhengqikj.top/gtfettslnc.html

[S29] C：变参函数
来源：http://hz.dianchejie.cn/gthzktzezs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtfmwfbzeq.html

[S30] C：头文件保护
来源：http://hz.sysykeji.top/gtroejwrle.html

#ifndef X_H
来源：http://hz.jianghu66.top/gtkbpxrowe.html

#define X_H
来源：http://hz.xinyue.icu/gtgbwxmzhx.html

#endif
来源：http://hz.xingfuxueyuan.xyz/gtwqboisbi.html

[S31] C++：Hello World
来源：http://hz.andypj.xyz/gtvvifkxyt.html

#include <iostream>
来源：http://hz.sweek.top/gtqunuvuse.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtmaxrgivt.html

[S32] C++：字符串
来源：http://hz.tianlin.xyz/gtegzaiqbp.html

std::string s = "hi";  s += "!";
来源：http://hz.zhixingplan.top/gttzclxvge.html

[S33] C++：vector 增删
来源：http://hz.andypj.xyz/gtjfpkyxjy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.nanxuanxn.top/gtpgrcjzch.html

[S34] C++：遍历 vector
来源：http://hz.jinqigufen.top/gtqijxdfch.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.nanxuanxn.top/gtpzxtdmnu.html

[S35] C++：map
来源：http://hz.gotoacloud.top/gtbewsgllh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tanke756.top/gtfrxrycgf.html

[S36] C++：unordered_map
来源：http://hz.shangyingyoupin.top/gtxqaowukq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtadjoynpa.html

[S37] C++：set
来源：http://hz.hywenlv.cn/gtbtwagydb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jlsjyb.cn/gtwfhtdzta.html

[S38] C++：排序
来源：http://hz.sxryk.cn/gtgspuxcpp.html

std::sort(v.begin(), v.end());
来源：http://hz.iojbl.cn/gtbmdimwdh.html

[S39] C++：自定义比较器排序
来源：http://hz.birdmap.top/gtjmatyulb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangshuangyany.cn/gtyngfqnoa.html

[S40] C++：查找元素
来源：http://hz.aibaodan.cn/gthpyunwii.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.aizwys.cn/gthanayrcv.html

[S41] C++：类与构造函数
来源：http://hz.iojbl.cn/gtdvbnivni.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jiagoushi.top/gtdgglmezc.html

[S42] C++：继承与虚函数
来源：http://hz.316326.xyz/gtydnkkvbg.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtdmztvgcs.html

[S43] C++：智能指针
来源：http://hz.yongpay.top/gtgivowgnw.html

auto p = std::make_unique<int>(5);
来源：http://hz.xziqi.cn/gtkutmcbjk.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtoetcetbs.html

void inc(int &x) { ++x; }
来源：http://hz.wangdashe.top/gtjfllonum.html

[S45] C++：lambda
来源：http://hz.birdmap.top/gtofpdqpuz.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aizwys.cn/gtlgnjrqtk.html

[S46] C++：函数模板
来源：http://hz.sxryk.cn/gtbpkrpwzu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.gogol.net.cn/gthobqeyzu.html

[S47] C++：结构化绑定遍历
来源：http://hz.yuxming.cn/gttnkgwhzl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gtjdccssde.html

[S48] C++：逐行读文件
来源：http://hz.yonumen.top/gtudnzcogd.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhixingplan.top/gtsjpdwrng.html

while (std::getline(in, line)) { }
来源：http://hz.yvedp.cn/gtxlxeltth.html

[S49] C++：写文件
来源：http://hz.snrcjt.cn/gtykmimybu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gtghypwotp.html

[S50] C++：格式化数字
来源：http://hz.feifeiyinyue.top/gtxotauvzh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.andypj.xyz/gtcggdgjaj.html

[S51] C++：显式类型转换
来源：http://hz.gzhubu.top/gtdilryuqu.html

static_cast<double>(a) / b
来源：http://hz.hfpthk.cn/gtxnvncbbu.html

[S52] C++：const 与 noexcept
来源：http://hz.c1oappe.top/gtipymxhbd.html

int size() const noexcept { return n_; }
来源：http://hz.hywenlv.cn/gtgjyzfphv.html

[S53] C++：移动语义
来源：http://hz.tianlin.xyz/gtwetdbvte.html

std::vector<int> w = std::move(v);
来源：http://hz.ywan-chungtsiang.top/gtrkvydozp.html

[S54] C++：异常处理
来源：http://hz.pengpengdd.cyou/gtvgzzacig.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.andypj.xyz/gthefdfgym.html

[S55] C++：结构化绑定
来源：http://hz.tian-w.cn/gtafltujth.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jiagoushi.top/gtqdtqpjwe.html

[S56] C++：optional
来源：http://hz.zhoulong.xyz/gtgxjnbbfs.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.gzhubu.top/gtxfrgyapa.html

[S57] C++：编译期常量
来源：http://hz.pengpengdd.cyou/gttuvytcbz.html

constexpr int N = 10;
来源：http://hz.meibo888.top/gtuzaovutj.html

[S58] C++：命名空间
来源：http://hz.meibo888.top/gtjjkohusr.html

namespace ns { int f() { return 1; } }
来源：http://hz.jinqigfzy.top/gttrtatldg.html

[S59] C++：静态断言
来源：http://hz.ywan-chungtsiang.top/gtgotspnjk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.sufxvd.cn/gtwlplzgny.html

[S60] C++：遍历并删除元素
来源：http://hz.meibo888.top/gtlmudmwmu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jyoumei.cn/gtiedryihm.html

================================================================================
来源：http://hz.nwbrower.top/gtlwflcthd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daxiang520.top/gtmtrjniml.html

================================================================================
来源：http://hz.yangfankeji.com/gtfacasjzu.html

[T01] Kotlin：Hello World
来源：http://hz.aizwys.cn/gtjvtgmhvv.html

println("Hello")
来源：http://hz.xylfe.cn/gtmfxpifay.html

[T02] Kotlin：变量
来源：http://hz.sweek.top/gtsfppexwp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ywan-chungtsiang.top/gtngrcibxq.html

[T03] Kotlin：字符串模板
来源：http://hz.316326.xyz/gtmticahxf.html

"值: $b"
来源：http://hz.daria6918.cn/gtyfwrntxy.html

[T04] Kotlin：空安全
来源：http://hz.yvedp.cn/gtjlzoncpb.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtwccozmbr.html

[T05] Kotlin：when 表达式
来源：http://hz.zdqjudy.top/gtymjgdysa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.feifeiyinyue.top/gtusfocnin.html

[T06] Kotlin：集合映射
来源：http://hz.jinqigufen.top/gtnpwbmanb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxuanxn.top/gtpspelgak.html

[T07] Kotlin：集合过滤
来源：http://hz.daxiang520.top/gtnglbtrrr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.tian-w.cn/gtzafdhchd.html

[T08] Kotlin：数据类
来源：http://hz.tian-w.cn/gtwzbeuzcn.html

data class User(val name: String, val age: Int)
来源：http://hz.smart0.xyz/gtyucrnrym.html

[T09] Kotlin：扩展函数
来源：http://hz.daxiang520.top/gtmipstxdx.html

fun String.exclaim() = this + "!"
来源：http://hz.gaohongyu789.top/gtlboozwzu.html

[T10] Kotlin：默认参数
来源：http://hz.zhongyouzk.top/gtwgxfjlrd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhijiandao.cn/gtvrpreywb.html

[T11] Kotlin：协程
来源：http://hz.cqqwz.cn/gtofecqafq.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xylfe.cn/gtmacprxmg.html

[T12] Kotlin：解构声明
来源：http://hz.dianchejie.cn/gttpanplyx.html

val (a, b) = Pair(1, 2)
来源：http://hz.zhijiandao.cn/gtyovlsuvq.html

[T13] Kotlin：只读 Map
来源：http://hz.jianghu66.top/gtjvmcqfia.html

val m = mapOf("a" to 1)
来源：http://hz.shanyushiyangtech.top/gtsvmgpktc.html

[T14] Kotlin：循环
来源：http://hz.gaohongyu789.top/gtxsgatpcl.html

for (i in 1..10) println(i)
来源：http://hz.yj20258.top/gtvckpmtpu.html

[T15] Kotlin：接口
来源：http://hz.ywan-chungtsiang.top/gtmepmiubv.html

interface Shape { fun area(): Double }
来源：http://hz.ivvv.top/gtipljpppp.html

[T16] Swift：Hello World
来源：http://hz.jlsjyb.cn/gtilqtxumy.html

print("Hello")
来源：http://hz.cqqwz.cn/gttyivhmhm.html

[T17] Swift：变量与常量
来源：http://hz.cqqwz.cn/gtsrxafxig.html

var a = 1;  let b = 2
来源：http://hz.pengpengdd.cyou/gtcvokribk.html

[T18] Swift：字符串插值
来源：http://hz.meibo888.top/gtvvjvplze.html

"值: \(b)"
来源：http://hz.yj20258.top/gttukyaqsw.html

[T19] Swift：可选绑定
来源：http://hz.gotoacloud.top/gtojtzznao.html

if let n = opt { print(n) }
来源：http://hz.pycfn.com/gtfzxweefv.html

[T20] Swift：数组操作
来源：http://hz.shuidangran.top/gtvvlxnrpe.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.aizwys.cn/gtoaesolfs.html

[T21] Swift：遍历
来源：http://hz.iojbl.cn/gtwwvuetvk.html

for x in a { print(x) }
来源：http://hz.shanyushiyangkeji.top/gtmqbyvbrs.html

[T22] Swift：字典
来源：http://hz.dashuyun.cn/gtyeeivagi.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.birdmap.top/gtfiquwiox.html

[T23] Swift：函数
来源：http://hz.chenlongwang.top/gtzdmtpiro.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.sweek.top/gtfmtfnlwr.html

[T24] Swift：闭包
来源：http://hz.andypj.xyz/gtwbzmjbhp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.wangdashe.top/gtxklnhcpv.html

[T25] Swift：结构体
来源：http://hz.sufxvd.cn/gtszdmjuzb.html

struct P { var x: Int }
来源：http://hz.sxryk.cn/gtmibonbkw.html

[T26] Swift：类与重写
来源：http://hz.havefunace.top/gtqmbcclqn.html

class A: Base { override func f() {} }
来源：http://hz.zycfv.cn/gtnniruxrr.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtffegjewm.html

do { try f() } catch { print(error) }
来源：http://hz.zhixingplan.top/gttijmjuep.html

[T28] Swift：枚举
来源：http://hz.yvedp.cn/gtseyzgsvt.html

enum Color { case red, green }
来源：http://hz.jinyuanbaomall.cn/gtwhvpckhb.html

[T29] Swift：guard 提前返回
来源：http://hz.hfpthk.cn/gtwnqsohkb.html

guard let x = opt else { return }
来源：http://hz.zhongyouzk.top/gtetutuaaz.html

[T30] Swift：协议
来源：http://hz.52xcode.cn/gtmipxjzlk.html

protocol Shape { func area() -> Double }
来源：http://hz.sweek.top/gtklblpvdj.html

[T31] Lua：Hello World
来源：http://hz.yj20258888.top/gtjywiveiq.html

print("Hello")
来源：http://hz.xinyue.icu/gtzuksgcbi.html

[T32] Lua：局部变量
来源：http://hz.hongshengwenyu.top/gtthhbfqxd.html

local a = 1
来源：http://hz.jqgfzy.top/gtuvvyglre.html

[T33] Lua：表（数组）
来源：http://hz.dashuyun.cn/gtyjtjtszg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.hywenlv.cn/gtakgufaqp.html

[T34] Lua：遍历表
来源：http://hz.tanke756.top/gthgixhefv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.zhaomingkeji.xyz/gtpwzvseai.html

[T35] Lua：字典表
来源：http://hz.birdmap.top/gtrkujwmda.html

local d = { a = 1 };  d.b = 2
来源：http://hz.gzhubu.top/gtottmqkfj.html

[T36] Lua：函数
来源：http://hz.daria6918.cn/gtrdbhowwm.html

function add(a, b) return a + b end
来源：http://hz.zhengqikj.top/gtsfxmruyh.html

[T37] Lua：字符串拼接
来源：http://hz.shzxlz.cn/gticbwnoqo.html

"a" .. "b"
来源：http://hz.shanyushiyangtech.top/gtjncdmgma.html

[T38] Lua：条件
来源：http://hz.zhixingplan.top/gtcwkluzfr.html

if x > 0 then print("正") end
来源：http://hz.jinyuanbaomall.cn/gtkgmzhehh.html

[T39] Lua：模式匹配
来源：http://hz.aibaodan.cn/gtisiduyjx.html

string.find(s, "%d+")
来源：http://hz.zhongyouzk.top/gtjxuxffzt.html

[T40] Lua：元表
来源：http://hz.yj20258.top/gtybudlmsy.html

setmetatable({}, { __index = base })
来源：http://hz.gotoacloud.top/gtaoaxoqjo.html

[T41] Perl：Hello World
来源：http://hz.gaohongyu789.top/gthktlzuvx.html

print "Hello\n";
来源：http://hz.52xcode.cn/gtpujuobjf.html

[T42] Perl：变量类型
来源：http://hz.shzxlz.cn/gtrjwgknxl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hz.yuxming.cn/gtyhibgcca.html


<!-- 参考信息 -->