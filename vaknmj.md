代发 wailian999

files=$(ls -1)
来源：http://hz.chenjidiqi.icu/gtyclozbxd.html

[R38] 管道串联
来源：http://hz.cdnleiting.top/gtsccenxgf.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhijiandao.cn/gttmgvdprq.html

[R39] 重定向标准输出与错误
来源：http://hz.xuanzx.com/gtngnbsrfu.html

cmd > out.log 2>&1
来源：http://hz.yonumen.top/gtmnczkqni.html

[R40] 追加写日志
来源：http://hz.xuanzx.com/gtniyjhvif.html

echo "log" >> out.log
来源：http://hz.chenlongwang.top/gtpocidqxv.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtccveyrka.html

cmd >/dev/null 2>&1
来源：http://hz.ydzc1.top/gtdqofewib.html

[R42] 输入重定向
来源：http://hz.316326.xyz/gtqpjsegfk.html

wc -l < a.txt
来源：http://hz.shanyushiyangtech.top/gtktkqaacj.html

[R43] 按名字查找文件
来源：http://hz.haohaochexian.top/gtqglxuimh.html

find . -name "*.log" -type f
来源：http://hz.gogol.net.cn/gtfgiiykuu.html

[R44] 按修改时间查找
来源：http://hz.cucudq.cn/gthfyqvhcn.html

find . -mtime -7 -type f
来源：http://hz.yuxming.cn/gtrubhzkwa.html

[R45] 批量删除
来源：http://hz.pycfn.com/gthdsqorkd.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtpsruuhmz.html

[R46] 递归替换文件内容
来源：http://hz.daria6918.cn/gtsrzumcmd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jlsjyb.cn/gtwbyrqkcn.html

[R47] sed 单行替换
来源：http://hz.shzxlz.cn/gtrwhyftqd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gthxbbjcil.html

[R48] awk 取指定列
来源：http://hz.cdnleiting.top/gtsovtrzka.html

awk '{print $1, $3}' a.txt
来源：http://hz.havefunace.top/gtzisgddlb.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gtdjzlnrta.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangdashe.top/gthxrfrpet.html

[R50] awk 求和
来源：http://hz.jqgfzy.top/gtyturcvnc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhiwuduotai.top/gtqxprkjbk.html

[R51] 排序去重取前几
来源：http://hz.wangshuangyany.cn/gtnvputcod.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xinyue.icu/gtabzsejrr.html

[R52] 统计行数
来源：http://hz.cucudq.cn/gthysxesok.html

wc -l a.txt
来源：http://hz.xingfuxueyuan.xyz/gtcwvjjllk.html

[R53] 查看文件头与实时尾
来源：http://hz.316326.xyz/gtczyksfjb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.andypj.xyz/gtrqebnxcs.html

[R54] 比较两个文件
来源：http://hz.ehwqpu.com/gtzngedlpt.html

diff a.txt b.txt
来源：http://hz.dianchejie.cn/gtfpwcejmf.html

[R55] 压缩与解压
来源：http://hz.wangshuangyany.cn/gtzqixlixa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.mhx1999.top/gtwqbobrxw.html

[R56] 远程拷贝
来源：http://hz.52xcode.cn/gtvksnfpos.html

scp file user@host:/path/
来源：http://hz.cqqwz.cn/gtmaonhwwp.html

[R57] 远程执行命令
来源：http://hz.yueranfly.top/gtacywwlje.html

ssh user@host 'uptime'
来源：http://hz.chenzaomai.com/gtohkomfig.html

[R58] 下载文件
来源：http://hz.dashuyun.cn/gtpghgkoyx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jianghu66.top/gtnkyvvhsf.html

[R59] 发 POST JSON
来源：http://hz.yongpay.top/gtwjgwsfeo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gtmoefgraq.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtkporceny.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jiagoushi.top/gtvibunsub.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gtqbifclgt.html

df -h;  du -sh *
来源：http://hz.zhoulong.xyz/gtwtxaekdk.html

[R62] 找最占空间的文件
来源：http://hz.yonumen.top/gtduvcvdib.html

du -ah . | sort -rh | head -10
来源：http://hz.xylfe.cn/gtvbzzwbmv.html

[R63] 内存与进程
来源：http://hz.0kj1m.cn/gtmqehpbko.html

free -h;  ps aux | grep nginx
来源：http://hz.zycfv.cn/gtcmvsrwry.html

[R64] 结束进程
来源：http://hz.ybcxt.top/gtqdutdpse.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtmpcvppwk.html

[R65] 查看端口占用
来源：http://hz.chenzaomai.com/gthwhugpyp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtrgpqndzs.html

[R66] 定时任务
来源：http://hz.hnxiangtu.top/gtmgxmtvie.html

crontab -e;  crontab -l
来源：http://hz.hysaishi.cn/gtppwydqsu.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtvlbycyzh.html

openssl rand -hex 16
来源：http://hz.yj202588.top/gtrtfmtkqd.html

[R68] 计算文件校验值
来源：http://hz.52xcode.cn/gtlcdjffzf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtaqhwajhg.html

[R69] 生成随机密码
来源：http://hz.yj20258888.top/gtmiuackew.html

head -c 16 /dev/urandom | base64
来源：http://hz.birdmap.top/gtavchthqs.html

[R70] 时间戳与互转
来源：http://hz.yonumen.top/gtkgvdmxlg.html

date +%s;  date -d @1700000000
来源：http://hz.jlsjyb.cn/gtgtwmwplv.html

[R71] 日期格式化
来源：http://hz.yanxiufei.cn/gtdzvmthhf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtpqcqlvcd.html

[R72] 等待端口就绪
来源：http://hz.hnqzz.top/gtsedzsopf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.andypj.xyz/gtrftsviwh.html

[R73] 分割大日志
来源：http://hz.zhengqikj.top/gtkmzqxxzj.html

split -l 1000 big.log part_
来源：http://hz.chenjidiqi.icu/gtqthiowbn.html

[R74] 批量重命名
来源：http://hz.hysaishi.cn/gtupjyggup.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnqzz.top/gtxeynfkdt.html

[R75] 导出环境变量
来源：http://hz.xuanzx.com/gtesrbwbiy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.aibaodan.cn/gtsvjknymf.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtxbnwdpsi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj20258.top/gttmyokthz.html

[R77] 读取用户输入
来源：http://hz.jinyuanbaomall.cn/gtowwupuij.html

read -rp "请输入: " ans
来源：http://hz.xziqi.cn/gtffgfdato.html

[R78] 交互式菜单
来源：http://hz.kuanghao11.cn/gtnfsfwnpl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigfzy.top/gtrmzjanoj.html

[R79] 解析命令行选项
来源：http://hz.316326.xyz/gteoyygrnf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gtrpakmyjj.html

[R80] 查看脚本执行耗时
来源：http://hz.daria6918.cn/gtduflslcj.html

time ./run.sh
来源：http://hz.chenzaomai.com/gtjlbbhmpd.html

================================================================================
来源：http://hz.jyoumei.cn/gtfuzrmxex.html

S. C / C++ 专题
来源：http://hz.sweek.top/gtmpgvxgyb.html

================================================================================
来源：http://hz.gaohongyu789.top/gtquszlhax.html

[S01] C：Hello World
来源：http://hz.sufxvd.cn/gtqkepegym.html

#include <stdio.h>
来源：http://hz.52xcode.cn/gtpghleyuy.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.shuidangran.top/gtjnnkgsse.html

[S02] C：变量与格式化输出
来源：http://hz.hfpthk.cn/gtfwontyzy.html

int a = 10; printf("%d\n", a);
来源：http://hz.iojbl.cn/gtklyztgsg.html

[S03] C：读入整数
来源：http://hz.cqqwz.cn/gtduijifub.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtdytwlsfp.html

[S04] C：字符串复制
来源：http://hz.zhaomingkeji.xyz/gtxfbguxzf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hammf.cn/gtvpahjhnb.html

[S05] C：字符串长度
来源：http://hz.bjfxy.top/gthnbpjovf.html

strlen(s)
来源：http://hz.jyoumei.cn/gtszpogpyc.html

[S06] C：字符串比较
来源：http://hz.jianghu66.top/gtxrztesxn.html

strcmp(a, b) == 0
来源：http://hz.sufxvd.cn/gtptyoivnp.html

[S07] C：数组遍历求和
来源：http://hz.guannengcc.top/gtvpvzurjr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hywenlv.cn/gtaejcjtvk.html

[S08] C：动态内存分配与释放
来源：http://hz.sxryk.cn/gtwfypycle.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gtwzjlqdjh.html

[S09] C：结构体定义与初始化
来源：http://hz.guowangkeji.top/gtnmgalhlk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangdashe.top/gtphnfclff.html

[S10] C：指针与解引用
来源：http://hz.xingfuxueyuan.xyz/gtkymtmohv.html

int *p = &a;  *p = 5;
来源：http://hz.yj202588.top/gtgiyeibdq.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtrmbyseab.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhaomingkeji.xyz/gtufceyfej.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ppjwa.cn/gtmecvnpxh.html

fclose(f);
来源：http://hz.daxiang520.top/gtumkoxlzw.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtwiyyecfv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.redwolf501.top/gtbqbiixln.html

[S13] C：宏定义
来源：http://hz.cheryme.top/gtewmlrtoz.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shangyingyoupin.top/gtopeaeaha.html

[S14] C：枚举
来源：http://hz.yuxming.cn/gtlosotdpx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhaomingkeji.xyz/gtsbbifbzi.html

[S15] C：类型转换
来源：http://hz.snrcjt.cn/gtpbyprajy.html

(double) a / b
来源：http://hz.nwbrower.top/gtoepkjofk.html

[S16] C：位操作置位
来源：http://hz.xingfuxueyuan.xyz/gtghkhixpf.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtbttyujrs.html

[S17] C：安全拼接字符串
来源：http://hz.gzhubu.top/gtzpbycfpj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenjidiqi.icu/gtnwoedhun.html

[S18] C：命令行参数
来源：http://hz.redwolf501.top/gtfesjfggk.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtdwipjjnx.html

[S19] C：快速排序
来源：http://hz.chenlongwang.top/gtjihgxotp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.havefunace.top/gtjarrwjgu.html

[S20] C：二分查找
来源：http://hz.hfpthk.cn/gttqljuzxp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.sweek.top/gtsrgajbbs.html

[S21] C：字符类别判断
来源：http://hz.tanke756.top/gtgoetykwu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.svipenyu.cn/gthewsntkj.html

[S22] C：字符串转数字
来源：http://hz.xinyue.icu/gtvskegccc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.jyoumei.cn/gtypfolexz.html

[S23] C：随机数
来源：http://hz.wangdashe.top/gtnjldehnn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ybcxt.top/gtjqpnqtqc.html

[S24] C：获取本地时间
来源：http://hz.aizwys.cn/gtpjncsodm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shangyingyoupin.top/gtvkyalxna.html

[S25] C：内存拷贝
来源：http://hz.jinqigufen.top/gtukoiqvsa.html

memcpy(dst, src, n);
来源：http://hz.cashguo.top/gtskogmdis.html

[S26] C：内存清零
来源：http://hz.9152youxi.cn/gtkwezgxmd.html

memset(a, 0, sizeof a);
来源：http://hz.dianchejie.cn/gtcqowjdlb.html

[S27] C：定义常量
来源：http://hz.andypj.xyz/gttkdjprui.html

const double PI = 3.14159;
来源：http://hz.gaohongyu789.top/gtgdadzggf.html

[S28] C：静态变量
来源：http://hz.pengpengdd.cyou/gtfulgkfbq.html

static int counter = 0;
来源：http://hz.jlsjyb.cn/gtjarqvcai.html

[S29] C：变参函数
来源：http://hz.yj20258.top/gtbuvtvkgr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.316326.xyz/gtxmkptukr.html

[S30] C：头文件保护
来源：http://hz.jinyuanbaomall.cn/gtqeudkwki.html

#ifndef X_H
来源：http://hz.shuidangran.top/gtbuvhcymh.html

#define X_H
来源：http://hz.jyoumei.cn/gtkliwkbhd.html

#endif
来源：http://hz.sxryk.cn/gtjiqzxqwn.html

[S31] C++：Hello World
来源：http://hz.fzhhl.top/gtivonrayk.html

#include <iostream>
来源：http://hz.tanke756.top/gtokiagofy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.9152youxi.cn/gttmfrcjul.html

[S32] C++：字符串
来源：http://hz.zhiwuduotai.top/gtecdmpumi.html

std::string s = "hi";  s += "!";
来源：http://hz.jqgfzy.top/gtzjmlucjr.html

[S33] C++：vector 增删
来源：http://hz.ydjk.org.cn/gtyawzyrox.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shanyushiyangkeji.top/gtbwwzzmcn.html

[S34] C++：遍历 vector
来源：http://hz.iojbl.cn/gtqljwjegh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daria6918.cn/gtjadipfjj.html

[S35] C++：map
来源：http://hz.feifeiyinyue.top/gtgadgzmtd.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtgdbutetr.html

[S36] C++：unordered_map
来源：http://hz.wangdashe.top/gtkccfklel.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.bjfxy.top/gtciebvzli.html

[S37] C++：set
来源：http://hz.316326.xyz/gtgsexuerx.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sweek.top/gtctzzphib.html

[S38] C++：排序
来源：http://hz.birdmap.top/gtslqmfifg.html

std::sort(v.begin(), v.end());
来源：http://hz.52xcode.cn/gtayevoien.html

[S39] C++：自定义比较器排序
来源：http://hz.nwbrower.top/gtrpxqjfep.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtdmjwyjyw.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtgrsnsils.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zhaomingkeji.xyz/gtneifhxiy.html

[S41] C++：类与构造函数
来源：http://hz.pengpengdd.cyou/gtbgaorpbj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtkpnasvvz.html

[S42] C++：继承与虚函数
来源：http://hz.chenjidiqi.icu/gtreqtfyjt.html

class B : public Base { public: void f() override {} };
来源：http://hz.gogol.net.cn/gtvhpjhfne.html

[S43] C++：智能指针
来源：http://hz.316326.xyz/gtryrfqnuk.html

auto p = std::make_unique<int>(5);
来源：http://hz.tianlin.xyz/gtbzciwgew.html

[S44] C++：引用传参
来源：http://hz.kuanghao11.cn/gtptvnccuz.html

void inc(int &x) { ++x; }
来源：http://hz.cucudq.cn/gtmrulthuy.html

[S45] C++：lambda
来源：http://hz.yangfankeji.com/gtjoeffyib.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhiwuduotai.top/gtaaunpkxa.html

[S46] C++：函数模板
来源：http://hz.ppjwa.cn/gtbvxvzbrk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhixingplan.top/gtwmzauajr.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gtjpkplhwq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xylfe.cn/gtvsapffcz.html

[S48] C++：逐行读文件
来源：http://hz.tanke756.top/gtfwfcfkmq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.xuetiantiany.cn/gtbmtmjxjm.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtnktnrlql.html

[S49] C++：写文件
来源：http://hz.pycfn.com/gtwshqrwfj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinghuilouyu.cn/gtciqkvvsx.html

[S50] C++：格式化数字
来源：http://hz.jyoumei.cn/gtqkzhywxr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtmlmtkzgg.html

[S51] C++：显式类型转换
来源：http://hz.316326.xyz/gtispdghmu.html

static_cast<double>(a) / b
来源：http://hz.dianchejie.cn/gtyzksldhs.html

[S52] C++：const 与 noexcept
来源：http://hz.chenzaomai.com/gtmptjvgag.html

int size() const noexcept { return n_; }
来源：http://hz.shzxlz.cn/gthxlkclpg.html

[S53] C++：移动语义
来源：http://hz.ehwqpu.com/gtdwnbafnc.html

std::vector<int> w = std::move(v);
来源：http://hz.chenjidiqi.icu/gtuftkamcq.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gthkbkinpv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.chenjidiqi.icu/gtfjzvjfbf.html

[S55] C++：结构化绑定
来源：http://hz.redwolf501.top/gtduedadyz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gtthszbgli.html

[S56] C++：optional
来源：http://hz.ydzc1.top/gtxkvlvkmh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.vqdsnc.cn/gtywwyknhz.html

[S57] C++：编译期常量
来源：http://hz.cashguo.top/gtwxbmvavi.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtmsgeexxs.html

[S58] C++：命名空间
来源：http://hz.wangdashe.top/gtjbnquxyn.html

namespace ns { int f() { return 1; } }
来源：http://hz.sysykeji.top/gtawgxrwte.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gtqgoutpmt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jianghu66.top/gtqlwcwoxe.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258.top/gtuufbazat.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.meibo888.top/gtnyfiqarb.html

================================================================================
来源：http://hz.ydzc1.top/gtwbcxtygd.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtmudeuwwr.html

================================================================================
来源：http://hz.316326.xyz/gttxsgltcv.html

[T01] Kotlin：Hello World
来源：http://hz.gogol.net.cn/gtaijhvvbu.html

println("Hello")
来源：http://hz.yvedp.cn/gttutovkwq.html

[T02] Kotlin：变量
来源：http://hz.jinqigufen.top/gtuwlcotsu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jqgufenzy.top/gtgulmlfyt.html

[T03] Kotlin：字符串模板
来源：http://hz.gzhubu.top/gtxzmsmsqc.html

"值: $b"
来源：http://hz.nwbrower.top/gtdwpzzzxk.html

[T04] Kotlin：空安全
来源：http://hz.jianghu66.top/gtzmmqeknd.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtaisejgnt.html

[T05] Kotlin：when 表达式
来源：http://hz.cdnleiting.top/gteoubzyga.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yuanzhike.top/gtoarqhmoc.html

[T06] Kotlin：集合映射
来源：http://hz.tian-w.cn/gtoefvvudk.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.wangdashe.top/gtnixxnvla.html

[T07] Kotlin：集合过滤
来源：http://hz.zhijiandao.cn/gtgtjcxalp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xuanzx.com/gtwchktnxp.html

[T08] Kotlin：数据类
来源：http://hz.shzxlz.cn/gtgaioyaxl.html

data class User(val name: String, val age: Int)
来源：http://hz.jiagoushi.top/gtfxftpdpc.html

[T09] Kotlin：扩展函数
来源：http://hz.shangyingyoupin.top/gtxrlmfzpv.html

fun String.exclaim() = this + "!"
来源：http://hz.ywan-chungtsiang.top/gtlxozmnwl.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtzdpuflfj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.tanke756.top/gtuakhploi.html

[T11] Kotlin：协程
来源：http://hz.wangdashe.top/gtepkxjfwk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dianchejie.cn/gtbfkisxqf.html

[T12] Kotlin：解构声明
来源：http://hz.mhx1999.top/gtplwdqqpl.html

val (a, b) = Pair(1, 2)
来源：http://hz.shangyingyoupin.top/gtwftfjiea.html

[T13] Kotlin：只读 Map
来源：http://hz.sweek.top/gtuvtullsk.html

val m = mapOf("a" to 1)
来源：http://hz.c1oappe.top/gtsizbrjuu.html

[T14] Kotlin：循环
来源：http://hz.zhijiandao.cn/gtnaabjnjm.html

for (i in 1..10) println(i)
来源：http://hz.svipenyu.cn/gtpwwufegu.html

[T15] Kotlin：接口
来源：http://hz.zhoulong.xyz/gttprwwuws.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtuddkxkgt.html

[T16] Swift：Hello World
来源：http://hz.tian-w.cn/gtvgqwmjvl.html

print("Hello")
来源：http://hz.ppjwa.cn/gtoaohhjmk.html

[T17] Swift：变量与常量
来源：http://hz.shzxlz.cn/gtvqquhpqh.html

var a = 1;  let b = 2
来源：http://hz.yanxiufei.cn/gtnbsjljlz.html

[T18] Swift：字符串插值
来源：http://hz.gotoacloud.top/gtgmystoff.html

"值: \(b)"
来源：http://hz.cqqwz.cn/gtslhadjsp.html

[T19] Swift：可选绑定
来源：http://hz.hammf.cn/gtxafvbemn.html

if let n = opt { print(n) }
来源：http://hz.guowangkeji.top/gtmrtmgqwk.html

[T20] Swift：数组操作
来源：http://hz.bjfxy.top/gtazesozmc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shangyingyoupin.top/gthgcqdffh.html

[T21] Swift：遍历
来源：http://hz.gaohongyu789.top/gtwzgilbbw.html

for x in a { print(x) }
来源：http://hz.xuanzx.com/gtyzhomtda.html

[T22] Swift：字典
来源：http://hz.smart0.xyz/gtznkjrovf.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jqgufenzy.top/gtziugwmkq.html

[T23] Swift：函数
来源：http://hz.yonumen.top/gtjsmsmqhe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.ywan-chungtsiang.top/gtkqrmbwyp.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtuajbgpom.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.cashguo.top/gtegxqpiuh.html

[T25] Swift：结构体
来源：http://hz.yuxming.cn/gtepmrkqvr.html

struct P { var x: Int }
来源：http://hz.havefunace.top/gtkmpgocwz.html

[T26] Swift：类与重写
来源：http://hz.pycfn.com/gtoninwsco.html

class A: Base { override func f() {} }
来源：http://hz.xziqi.cn/gtcngdplfo.html

[T27] Swift：错误处理
来源：http://hz.birdmap.top/gtnthpnnvg.html

do { try f() } catch { print(error) }
来源：http://hz.yueranfly.top/gtpzvvtdjo.html

[T28] Swift：枚举
来源：http://hz.ppjwa.cn/gtfmbrdkgm.html

enum Color { case red, green }
来源：http://hz.zhongyouzk.top/gtxnftjnsr.html

[T29] Swift：guard 提前返回
来源：http://hz.feifeiyinyue.top/gtbnwfqrtq.html

guard let x = opt else { return }
来源：http://hz.hfpthk.cn/gtybqqumeu.html

[T30] Swift：协议
来源：http://hz.hnxiangtu.top/gtomjuyzaf.html

protocol Shape { func area() -> Double }
来源：http://hz.yueranfly.top/gtaipjznyc.html

[T31] Lua：Hello World
来源：http://hz.nwbrower.top/gtgnnoinqv.html

print("Hello")
来源：http://hz.pengpengdd.cyou/gtpssqvqvl.html

[T32] Lua：局部变量
来源：http://hz.feifeiyinyue.top/gtddrktctd.html

local a = 1
来源：http://hz.daxiang520.top/gtbvxriemj.html

[T33] Lua：表（数组）
来源：http://hz.nwbrower.top/gtyntwwakw.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.zhijiandao.cn/gtbunzoods.html

[T34] Lua：遍历表
来源：http://hz.havefunace.top/gtbpatsumg.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.haohaochexian.top/gtjfibnbcs.html

[T35] Lua：字典表
来源：http://hz.tian-w.cn/gtocujvabk.html

local d = { a = 1 };  d.b = 2
来源：http://hz.xingfuxueyuan.xyz/gtjwyxtkvf.html

[T36] Lua：函数
来源：http://hz.jyoumei.cn/gtinuftrch.html

function add(a, b) return a + b end
来源：http://hz.c1oappe.top/gtpvizuloe.html

[T37] Lua：字符串拼接
来源：http://hz.ydzc1.top/gtnoxrogyz.html

"a" .. "b"
来源：http://hz.shzxlz.cn/gtwwrqnhjw.html

[T38] Lua：条件
来源：http://hz.0kj1m.cn/gtnagekcno.html

if x > 0 then print("正") end
来源：http://hz.gotoacloud.top/gtjsbwihla.html

[T39] Lua：模式匹配
来源：http://hz.zhixingplan.top/gtzbltarlm.html

string.find(s, "%d+")
来源：http://hz.quarkkingdee.top/gtyrfqfnjq.html

[T40] Lua：元表
来源：http://hz.sysykeji.top/gttsiqrzav.html

setmetatable({}, { __index = base })
来源：http://hz.kuanghao11.cn/gtfzjrvemf.html


<!-- 参考信息 -->