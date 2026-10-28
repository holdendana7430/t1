代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hongshengwenyu.top/gtuzpgyhzm.html

[R30] 函数返回状态码
来源：http://hz.yuxming.cn/gtnlhexrxc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.meibo888.top/gtbturdyap.html

[R31] 局部变量
来源：http://hz.chenjidiqi.icu/gtziptbzob.html

f() { local x=1; echo "$x"; }
来源：http://hz.zycfv.cn/gtwqjyeevv.html

[R32] 参数个数校验
来源：http://hz.aizwys.cn/gtpgxkzbmj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jianghu66.top/gtkbvafmyl.html

[R33] 捕获错误并提示行号
来源：http://hz.316326.xyz/gthzljowql.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.c1oappe.top/gtvcgzhbqf.html

[R34] 退出时清理
来源：http://hz.xuetiantiany.cn/gtjllyxpyk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jiagoushi.top/gtkhkxdhsa.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtuigogqkb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhijiandao.cn/gtjevqueco.html

[R36] 并发执行多个任务
来源：http://hz.birdmap.top/gtyisccamq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gteroiowhv.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtybilrann.html

files=$(ls -1)
来源：http://hz.tian-w.cn/gtjhlfxpwv.html

[R38] 管道串联
来源：http://hz.ybcxt.top/gtzwpvwkze.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtaonkpypx.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258888.top/gtbvvlmrsi.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gttqmrrfnr.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtjyyqrfzx.html

echo "log" >> out.log
来源：http://hz.zhongyouzk.top/gtslmwshiw.html

[R41] 丢弃输出
来源：http://hz.jianghu66.top/gtxkqyksye.html

cmd >/dev/null 2>&1
来源：http://hz.shanyushiyangkeji.top/gtynucllxh.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtljydecyx.html

wc -l < a.txt
来源：http://hz.yanxiufei.cn/gtivvscioo.html

[R43] 按名字查找文件
来源：http://hz.52xcode.cn/gtugzpvzlf.html

find . -name "*.log" -type f
来源：http://hz.shanyushiyangkeji.top/gtuutevhie.html

[R44] 按修改时间查找
来源：http://hz.316326.xyz/gttdilrvwd.html

find . -mtime -7 -type f
来源：http://hz.feifeiyinyue.top/gtkwgaikir.html

[R45] 批量删除
来源：http://hz.guannengcc.top/gtjrjbatho.html

find . -name "*.tmp" -delete
来源：http://hz.xylfe.cn/gtfbfnsbnc.html

[R46] 递归替换文件内容
来源：http://hz.ehwqpu.com/gtsseifcqc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtmpcmzgza.html

[R47] sed 单行替换
来源：http://hz.quarkkingdee.top/gtkqljgnnp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.pycfn.com/gtznaanpst.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtxrzkrxtf.html

awk '{print $1, $3}' a.txt
来源：http://hz.ydjk.org.cn/gtynrlidcu.html

[R49] awk 带条件
来源：http://hz.sysykeji.top/gtcrlourjc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cqqwz.cn/gtwlnpieoq.html

[R50] awk 求和
来源：http://hz.hnxiangtu.top/gthfaubihe.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.xziqi.cn/gtulpqdlbf.html

[R51] 排序去重取前几
来源：http://hz.9152youxi.cn/gtakcherlk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangdashe.top/gttovupaeu.html

[R52] 统计行数
来源：http://hz.meibo888.top/gtqljdvfuc.html

wc -l a.txt
来源：http://hz.nanxinkj.top/gtvpxesmpe.html

[R53] 查看文件头与实时尾
来源：http://hz.dashuyun.cn/gtvhariaoi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangshuangyany.cn/gtokelnxcr.html

[R54] 比较两个文件
来源：http://hz.yanxiufei.cn/gtadpmipow.html

diff a.txt b.txt
来源：http://hz.yvedp.cn/gtltoeammd.html

[R55] 压缩与解压
来源：http://hz.vqdsnc.cn/gtiheauizg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.svipenyu.cn/gtalzjrfly.html

[R56] 远程拷贝
来源：http://hz.cucudq.cn/gtlkxbsasc.html

scp file user@host:/path/
来源：http://hz.xinyue.icu/gtnrdbktsq.html

[R57] 远程执行命令
来源：http://hz.gogol.net.cn/gteudhesui.html

ssh user@host 'uptime'
来源：http://hz.sysykeji.top/gtluctecjy.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtzjkdytrv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ydzc1.top/gthwlzjnac.html

[R59] 发 POST JSON
来源：http://hz.guowangkeji.top/gtwpfsikml.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.xziqi.cn/gtbgolfsuk.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtdjlichla.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.316326.xyz/gtvupxdqxs.html

[R61] 磁盘占用
来源：http://hz.chenzaomai.com/gtbspwrexb.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gtwtvjjyns.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtlgakduhq.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxinkj.top/gtvlzmebvz.html

[R63] 内存与进程
来源：http://hz.sweek.top/gtdbrdctno.html

free -h;  ps aux | grep nginx
来源：http://hz.svipenyu.cn/gtcnfjierm.html

[R64] 结束进程
来源：http://hz.chenlongwang.top/gtbiqttafi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.bjfxy.top/gtuceirlyq.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtelvorbkk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtpiffxcuz.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtmaddmycl.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gtswobegpu.html

[R67] 生成随机十六进制串
来源：http://hz.xziqi.cn/gtpgkysjrn.html

openssl rand -hex 16
来源：http://hz.yonumen.top/gtbvfcftgu.html

[R68] 计算文件校验值
来源：http://hz.nwbrower.top/gtepiskvor.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.guannengcc.top/gtvzlwavai.html

[R69] 生成随机密码
来源：http://hz.dianchejie.cn/gtotguzvmf.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtpsvdlesn.html

[R70] 时间戳与互转
来源：http://hz.chenzaomai.com/gtmyyygbkz.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtmfajqhkh.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtmkjdgubw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daria6918.cn/gtnkdxkidy.html

[R72] 等待端口就绪
来源：http://hz.9152youxi.cn/gtmpoklswm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhijiandao.cn/gttzkbixsw.html

[R73] 分割大日志
来源：http://hz.yuanzhike.top/gtmizfeoua.html

split -l 1000 big.log part_
来源：http://hz.hongshengwenyu.top/gtnkbncact.html

[R74] 批量重命名
来源：http://hz.xingfuxueyuan.xyz/gtmspmwjaq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fengsongda.top/gtcjrqupae.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtkaxcguso.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pycfn.com/gtnasccpgo.html

[R76] 使用临时文件
来源：http://hz.yuxming.cn/gtjfgmedhl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtjmiujlhj.html

[R77] 读取用户输入
来源：http://hz.jqgfzy.top/gtvxzkzwap.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtrxgfeuxk.html

[R78] 交互式菜单
来源：http://hz.sxryk.cn/gtjitdaxif.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.smart0.xyz/gtkglwqbze.html

[R79] 解析命令行选项
来源：http://hz.52xcode.cn/gtxdjtelqi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.chenlongwang.top/gthvooykuw.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gtqskshzrx.html

time ./run.sh
来源：http://hz.yanxiufei.cn/gtitjlccbi.html

================================================================================
来源：http://hz.aizwys.cn/gtosvlbcxx.html

S. C / C++ 专题
来源：http://hz.havefunace.top/gtxnjnmjki.html

================================================================================
来源：http://hz.hywenlv.cn/gtaqnoxvxe.html

[S01] C：Hello World
来源：http://hz.yangfankeji.com/gtcjcnnryr.html

#include <stdio.h>
来源：http://hz.jinqigfzy.top/gtfcudehia.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.mhx1999.top/gtfipdfhxg.html

[S02] C：变量与格式化输出
来源：http://hz.haohaochexian.top/gtadhkfhbp.html

int a = 10; printf("%d\n", a);
来源：http://hz.nanxinkj.top/gttttceway.html

[S03] C：读入整数
来源：http://hz.ivvv.top/gtdqduypdx.html

int x; scanf("%d", &x);
来源：http://hz.ehwqpu.com/gtluiyolun.html

[S04] C：字符串复制
来源：http://hz.ywan-chungtsiang.top/gtjwqtajhh.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cqqwz.cn/gtbpvjdmzw.html

[S05] C：字符串长度
来源：http://hz.yj20258.top/gtfugwlzzs.html

strlen(s)
来源：http://hz.sweek.top/gtttktywny.html

[S06] C：字符串比较
来源：http://hz.0kj1m.cn/gtkzkoiwwe.html

strcmp(a, b) == 0
来源：http://hz.ehwqpu.com/gtlbylrqzb.html

[S07] C：数组遍历求和
来源：http://hz.hywenlv.cn/gtajxfoiyf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zdqjudy.top/gtuqbupjwm.html

[S08] C：动态内存分配与释放
来源：http://hz.sweek.top/gtsbffevst.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtcgwfhpkp.html

[S09] C：结构体定义与初始化
来源：http://hz.vqdsnc.cn/gtwsxcjsfy.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hfpthk.cn/gtdgqeqjwr.html

[S10] C：指针与解引用
来源：http://hz.0kj1m.cn/gtexifhldl.html

int *p = &a;  *p = 5;
来源：http://hz.birdmap.top/gtpwlrgpvu.html

[S11] C：逐行读文件
来源：http://hz.52xcode.cn/gtaystacfn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jlsjyb.cn/gtpxbuqxqg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gtgrylljqg.html

fclose(f);
来源：http://hz.yuxming.cn/gtrhyecqrc.html

[S12] C：写文件
来源：http://hz.yonumen.top/gtlpiguxfu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zycfv.cn/gtazyeucic.html

[S13] C：宏定义
来源：http://hz.hysaishi.cn/gtyehwhfcg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.bjfxy.top/gtrrlgekda.html

[S14] C：枚举
来源：http://hz.daxiang520.top/gtbteajcrm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.quarkkingdee.top/gtnwytzmfe.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtgszwxuys.html

(double) a / b
来源：http://hz.nanxinkj.top/gtyskmjuwh.html

[S16] C：位操作置位
来源：http://hz.xinyue.icu/gtqzmoooso.html

x |= (1 << 3);
来源：http://hz.hfpthk.cn/gtimvhxegp.html

[S17] C：安全拼接字符串
来源：http://hz.shanyushiyangtech.top/gtnxwegehz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtwzokxaye.html

[S18] C：命令行参数
来源：http://hz.tian-w.cn/gtbjrypmni.html

int main(int argc, char **argv)
来源：http://hz.meibo888.top/gtqjtblvuv.html

[S19] C：快速排序
来源：http://hz.sxryk.cn/gthpdvdtgh.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yueranfly.top/gtxtqhnfsk.html

[S20] C：二分查找
来源：http://hz.jinghuilouyu.cn/gtxogmiokk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.aibaodan.cn/gtwmrrrmgj.html

[S21] C：字符类别判断
来源：http://hz.andypj.xyz/gtmqzaxdfu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gtpzfgcacb.html

[S22] C：字符串转数字
来源：http://hz.fzhhl.top/gtwnzdyxeh.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hysaishi.cn/gtvujerfav.html

[S23] C：随机数
来源：http://hz.bjfxy.top/gtohvbnlrn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.ppjwa.cn/gtfwjvxjau.html

[S24] C：获取本地时间
来源：http://hz.guowangkeji.top/gtzzbecbgo.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.gzhubu.top/gtybsdnqev.html

[S25] C：内存拷贝
来源：http://hz.jinyuanbaomall.cn/gtbzaerujf.html

memcpy(dst, src, n);
来源：http://hz.shangyingyoupin.top/gtbuqjomvo.html

[S26] C：内存清零
来源：http://hz.snrcjt.cn/gtmfzynijs.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtonpramgi.html

[S27] C：定义常量
来源：http://hz.zycfv.cn/gtqiwkubee.html

const double PI = 3.14159;
来源：http://hz.chenzaomai.com/gthzgxdfha.html

[S28] C：静态变量
来源：http://hz.xuanzx.com/gtbxdxukgk.html

static int counter = 0;
来源：http://hz.jiagoushi.top/gtoiqwphsk.html

[S29] C：变参函数
来源：http://hz.jinqigfzy.top/gtlgalsyvd.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.kuanghao11.cn/gtgzpedjny.html

[S30] C：头文件保护
来源：http://hz.chenjidiqi.icu/gttmvswows.html

#ifndef X_H
来源：http://hz.haohaochexian.top/gtswqmozph.html

#define X_H
来源：http://hz.ydzc1.top/gttveytslr.html

#endif
来源：http://hz.andypj.xyz/gtlagtlirs.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtlgtmttgp.html

#include <iostream>
来源：http://hz.havefunace.top/gtixxfodza.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.svipenyu.cn/gtmvggtwyd.html

[S32] C++：字符串
来源：http://hz.tian-w.cn/gtelpujlzj.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtrowiowib.html

[S33] C++：vector 增删
来源：http://hz.xylfe.cn/gtcgodgrrn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ehwqpu.com/gteqchsscg.html

[S34] C++：遍历 vector
来源：http://hz.shanyushiyangtech.top/gtezblywiq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jqgfzy.top/gttpzygemu.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtnatgbdxs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtbyanfwlz.html

[S36] C++：unordered_map
来源：http://hz.yj20258888.top/gtgkhbsoyd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.iojbl.cn/gtasuaawgu.html

[S37] C++：set
来源：http://hz.xuetiantiany.cn/gtkzbpkmsd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jinqigfzy.top/gtptdvahkh.html

[S38] C++：排序
来源：http://hz.pengpengdd.cyou/gtmnwivwuv.html

std::sort(v.begin(), v.end());
来源：http://hz.gotoacloud.top/gtiljbfqia.html

[S39] C++：自定义比较器排序
来源：http://hz.yvedp.cn/gtzemhtkfe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.chenlongwang.top/gtoqsxklxs.html

[S40] C++：查找元素
来源：http://hz.shanyushiyangkeji.top/gtrmorjedo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangkeji.top/gtqqxftqtr.html

[S41] C++：类与构造函数
来源：http://hz.hywenlv.cn/gtognatmzb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhaomingkeji.xyz/gttzslgrtp.html

[S42] C++：继承与虚函数
来源：http://hz.ehwqpu.com/gtxhnyivre.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuanzhike.top/gtzvbaiufu.html

[S43] C++：智能指针
来源：http://hz.9152youxi.cn/gtszwdcnuf.html

auto p = std::make_unique<int>(5);
来源：http://hz.xinyue.icu/gtmgarfbnb.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtnaspnlao.html

void inc(int &x) { ++x; }
来源：http://hz.yueranfly.top/gtfsjpxuaq.html

[S45] C++：lambda
来源：http://hz.guannengcc.top/gtgtnuienm.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtufzwldcu.html

[S46] C++：函数模板
来源：http://hz.cashguo.top/gtphppeezi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenjidiqi.icu/gtnbgatqyf.html

[S47] C++：结构化绑定遍历
来源：http://hz.yueranfly.top/gttnulqkkw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.iojbl.cn/gtxdggvxkl.html

[S48] C++：逐行读文件
来源：http://hz.zhongyouzk.top/gtppbloaze.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.chenzaomai.com/gtbnnfyghy.html

while (std::getline(in, line)) { }
来源：http://hz.hfpthk.cn/gtwaobsohh.html

[S49] C++：写文件
来源：http://hz.xuanzx.com/gtsgbbwpbg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhongyouzk.top/gtdoxysopm.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtyoywjgej.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.tian-w.cn/gtnhxgfzrk.html

[S51] C++：显式类型转换
来源：http://hz.fzhhl.top/gtadexpswv.html

static_cast<double>(a) / b
来源：http://hz.jqgufenzy.top/gtnljwvgji.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtfuolzgue.html

int size() const noexcept { return n_; }
来源：http://hz.wangdashe.top/gtlctvbqld.html

[S53] C++：移动语义
来源：http://hz.aibaodan.cn/gtdipivbmx.html

std::vector<int> w = std::move(v);
来源：http://hz.svipenyu.cn/gtyzvpnklk.html

[S54] C++：异常处理
来源：http://hz.zhixingplan.top/gtprflvhzl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yuanzhike.top/gtkllanetd.html

[S55] C++：结构化绑定
来源：http://hz.snrcjt.cn/gtkriigxug.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtvoxfgrxd.html

[S56] C++：optional
来源：http://hz.zycfv.cn/gtuwwihhah.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtbcdnwtor.html

[S57] C++：编译期常量
来源：http://hz.jianghu66.top/gtxeixjjkr.html

constexpr int N = 10;
来源：http://hz.pengpengdd.cyou/gtsehghsvk.html

[S58] C++：命名空间
来源：http://hz.shzxlz.cn/gtovioanst.html

namespace ns { int f() { return 1; } }
来源：http://hz.guannengcc.top/gtghjnffpd.html

[S59] C++：静态断言
来源：http://hz.0kj1m.cn/gthjbwdzed.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhengqikj.top/gtozenixnm.html

[S60] C++：遍历并删除元素
来源：http://hz.nwbrower.top/gtdrtkyota.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.iojbl.cn/gtpxscntfd.html

================================================================================
来源：http://hz.shuidangran.top/gtbztwjwwf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhoulong.xyz/gteoujecjm.html

================================================================================
来源：http://hz.vqdsnc.cn/gtnyvsmang.html

[T01] Kotlin：Hello World
来源：http://hz.cheryme.top/gtxzhesdqu.html

println("Hello")
来源：http://hz.xuanzx.com/gthbmlbxsj.html

[T02] Kotlin：变量
来源：http://hz.wangdashe.top/gtvqmpvvwf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.chenlongwang.top/gtymjydzcd.html

[T03] Kotlin：字符串模板
来源：http://hz.smart0.xyz/gtikooanut.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtwdaliyxf.html

[T04] Kotlin：空安全
来源：http://hz.tian-w.cn/gtrwpkqmtt.html

val n: String? = null;  n?.length
来源：http://hz.yj202588.top/gtloqputxq.html

[T05] Kotlin：when 表达式
来源：http://hz.feifeiyinyue.top/gtnklbjlic.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yj202588.top/gtnrunwutw.html

[T06] Kotlin：集合映射
来源：http://hz.mhx1999.top/gtvyvnrzia.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yj202588.top/gtuevoqnbg.html

[T07] Kotlin：集合过滤
来源：http://hz.shangyingyoupin.top/gtodjprvdw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zdqjudy.top/gtqdazqouk.html

[T08] Kotlin：数据类
来源：http://hz.zhiwuduotai.top/gtrycmghvp.html

data class User(val name: String, val age: Int)
来源：http://hz.cucudq.cn/gtjisktltn.html

[T09] Kotlin：扩展函数
来源：http://hz.iojbl.cn/gtvmatczvu.html

fun String.exclaim() = this + "!"
来源：http://hz.yvedp.cn/gteywmwnlk.html

[T10] Kotlin：默认参数
来源：http://hz.ivvv.top/gtimrrpbld.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zycfv.cn/gtcafjnydm.html

[T11] Kotlin：协程
来源：http://hz.ivvv.top/gtzjewbcwr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.hnqzz.top/gtzyhxrimv.html

[T12] Kotlin：解构声明
来源：http://hz.shanyushiyangkeji.top/gtaoywrhvl.html

val (a, b) = Pair(1, 2)
来源：http://hz.hfpthk.cn/gtovigdcny.html

[T13] Kotlin：只读 Map
来源：http://hz.feifeiyinyue.top/gtkinbdlxq.html

val m = mapOf("a" to 1)
来源：http://hz.yvedp.cn/gtmvklozer.html

[T14] Kotlin：循环
来源：http://hz.shzxlz.cn/gtaqjzckul.html

for (i in 1..10) println(i)
来源：http://hz.nanxinkj.top/gtoynuwwkz.html

[T15] Kotlin：接口
来源：http://hz.shanyushiyangtech.top/gtqrmffldp.html

interface Shape { fun area(): Double }
来源：http://hz.chenjidiqi.icu/gtulqmztyb.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtjuichrur.html

print("Hello")
来源：http://hz.ywan-chungtsiang.top/gtcndiaacz.html

[T17] Swift：变量与常量
来源：http://hz.zhiwuduotai.top/gtydwaksyq.html

var a = 1;  let b = 2
来源：http://hz.yonumen.top/gtdofkxdiu.html

[T18] Swift：字符串插值
来源：http://hz.xylfe.cn/gtseqddpmj.html

"值: \(b)"
来源：http://hz.tanke756.top/gthtlaofbu.html

[T19] Swift：可选绑定
来源：http://hz.andypj.xyz/gtptaeluup.html

if let n = opt { print(n) }
来源：http://hz.cheryme.top/gtdcnxpnax.html

[T20] Swift：数组操作
来源：http://hz.c1oappe.top/gtedqwwfnx.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.mhx1999.top/gtwkazmnwx.html

[T21] Swift：遍历
来源：http://hz.fzhhl.top/gtqrictsxa.html

for x in a { print(x) }
来源：http://hz.hysaishi.cn/gtmdlhkdem.html

[T22] Swift：字典
来源：http://hz.yuxming.cn/gtigkifgci.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.andypj.xyz/gtdoiaeowd.html

[T23] Swift：函数
来源：http://hz.pycfn.com/gtazwmeifo.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.kuanghao11.cn/gtyhxyqczq.html

[T24] Swift：闭包
来源：http://hz.cqqwz.cn/gturlvbllr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.guowangkeji.top/gtungviozy.html

[T25] Swift：结构体
来源：http://hz.jinqigufen.top/gttiuwovzd.html

struct P { var x: Int }
来源：http://hz.jqgufenzy.top/gtvjxeoazq.html

[T26] Swift：类与重写
来源：http://hz.ehwqpu.com/gtglifiryt.html

class A: Base { override func f() {} }
来源：http://hz.ywan-chungtsiang.top/gtrmnsepoy.html

[T27] Swift：错误处理
来源：http://hz.wangdashe.top/gtypkjahor.html

do { try f() } catch { print(error) }
来源：http://hz.chenlongwang.top/gtvutqugjy.html

[T28] Swift：枚举
来源：http://hz.cucudq.cn/gtmeqzzjoa.html

enum Color { case red, green }
来源：http://hz.pengpengdd.cyou/gtlkkfhfqn.html

[T29] Swift：guard 提前返回
来源：http://hz.wangshuangyany.cn/gtqmpmghem.html

guard let x = opt else { return }
来源：http://hz.smart0.xyz/gtefswdfal.html

[T30] Swift：协议
来源：http://hz.yanxiufei.cn/gtoumxzram.html

protocol Shape { func area() -> Double }
来源：http://hz.zhongyouzk.top/gtnvpuclts.html

[T31] Lua：Hello World
来源：http://hz.yj202588.top/gtxxjbqsuo.html

print("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtvchpjyak.html

[T32] Lua：局部变量
来源：http://hz.yangfankeji.com/gtbffztegf.html

local a = 1
来源：http://hz.sysykeji.top/gtrygdzpgh.html


<!-- 参考信息 -->