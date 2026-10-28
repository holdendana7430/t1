代发 wailian999

f() { local x=1; echo "$x"; }
来源：http://hz.cdnleiting.top/gtrsjepbsi.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtkdeoxoqb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hysaishi.cn/gtpbovkgzp.html

[R33] 捕获错误并提示行号
来源：http://hz.xuanzx.com/gtzczkgrue.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yangfankeji.com/gtpzfgnlhr.html

[R34] 退出时清理
来源：http://hz.jinghuilouyu.cn/gthhbnhgkt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hammf.cn/gtltidgfpu.html

[R35] 后台执行并等待
来源：http://hz.pycfn.com/gtkrapmljn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yanxiufei.cn/gtnqfezuyd.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gtbcwmatjh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pycfn.com/gtikbaidzd.html

[R37] 把输出赋给变量
来源：http://hz.shangyingyoupin.top/gtnrqwxlvp.html

files=$(ls -1)
来源：http://hz.hammf.cn/gtuhqdbeoq.html

[R38] 管道串联
来源：http://hz.zhixingplan.top/gtxvfnzjbt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aibaodan.cn/gtdsrtlbti.html

[R39] 重定向标准输出与错误
来源：http://hz.andypj.xyz/gtdbddadbj.html

cmd > out.log 2>&1
来源：http://hz.hnxiangtu.top/gtdqcxmrtp.html

[R40] 追加写日志
来源：http://hz.yangfankeji.com/gtohncftij.html

echo "log" >> out.log
来源：http://hz.shanyushiyangkeji.top/gtoleucanz.html

[R41] 丢弃输出
来源：http://hz.aibaodan.cn/gtuxzdujtk.html

cmd >/dev/null 2>&1
来源：http://hz.cqqwz.cn/gtprgsfnnh.html

[R42] 输入重定向
来源：http://hz.gotoacloud.top/gtpeoqtjgf.html

wc -l < a.txt
来源：http://hz.havefunace.top/gtnzsfumfs.html

[R43] 按名字查找文件
来源：http://hz.yonumen.top/gtmbrdsdfn.html

find . -name "*.log" -type f
来源：http://hz.ybcxt.top/gtwmtpuqsy.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtgcejytdt.html

find . -mtime -7 -type f
来源：http://hz.feifeiyinyue.top/gtrychtibk.html

[R45] 批量删除
来源：http://hz.yuxming.cn/gtcpuhxqaq.html

find . -name "*.tmp" -delete
来源：http://hz.sweek.top/gtmmewnhpl.html

[R46] 递归替换文件内容
来源：http://hz.ywan-chungtsiang.top/gtohzpfops.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shanyushiyangkeji.top/gtproxrmid.html

[R47] sed 单行替换
来源：http://hz.zycfv.cn/gtltwmwwxa.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtxfhpvtjl.html

[R48] awk 取指定列
来源：http://hz.sysykeji.top/gtqembexsl.html

awk '{print $1, $3}' a.txt
来源：http://hz.hysaishi.cn/gtuqykvjlz.html

[R49] awk 带条件
来源：http://hz.yj20258888.top/gtrkwohzwh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhijiandao.cn/gtqydvgfem.html

[R50] awk 求和
来源：http://hz.ehwqpu.com/gtrpqrhgph.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tianlin.xyz/gtjknnvotp.html

[R51] 排序去重取前几
来源：http://hz.gzhubu.top/gtschhqgyw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.xingfuxueyuan.xyz/gtmafpixxw.html

[R52] 统计行数
来源：http://hz.hnqzz.top/gtfqznwnwi.html

wc -l a.txt
来源：http://hz.nanxinkj.top/gtrrritoex.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gtzzwmudtk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.andypj.xyz/gtezeajkgr.html

[R54] 比较两个文件
来源：http://hz.zhijiandao.cn/gtkyyqxlkg.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtbhjgcqoh.html

[R55] 压缩与解压
来源：http://hz.ywan-chungtsiang.top/gtzqvjqzlb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gtdnrniuxn.html

[R56] 远程拷贝
来源：http://hz.ybcxt.top/gtzkjgzwca.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gtwttwxbaq.html

[R57] 远程执行命令
来源：http://hz.yj20258888.top/gtpctkfkfa.html

ssh user@host 'uptime'
来源：http://hz.pycfn.com/gthveqkbor.html

[R58] 下载文件
来源：http://hz.mhx1999.top/gtjdhywekf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtfvwsvzcp.html

[R59] 发 POST JSON
来源：http://hz.gotoacloud.top/gtqmtrnmwy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cashguo.top/gtylrkebqs.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenzaomai.com/gtkpooqqjn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtqbdlgrja.html

[R61] 磁盘占用
来源：http://hz.shanyushiyangtech.top/gtmfzbwbnk.html

df -h;  du -sh *
来源：http://hz.haohaochexian.top/gtkyxyrlgo.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gtdicvzqur.html

du -ah . | sort -rh | head -10
来源：http://hz.xingfuxueyuan.xyz/gtfylqcbqi.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gtorckijlv.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtuhjfwqhd.html

[R64] 结束进程
来源：http://hz.yj20258.top/gtyjqugqvb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xinyue.icu/gtdkljocit.html

[R65] 查看端口占用
来源：http://hz.redwolf501.top/gthkwiotoy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yuanzhike.top/gtgwarsshe.html

[R66] 定时任务
来源：http://hz.pengpengdd.cyou/gtlovcfmki.html

crontab -e;  crontab -l
来源：http://hz.gogol.net.cn/gtcexspgcp.html

[R67] 生成随机十六进制串
来源：http://hz.andypj.xyz/gtlyskhnel.html

openssl rand -hex 16
来源：http://hz.zhongyouzk.top/gtouchycge.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gtyaydxbjv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuanzhike.top/gtglhpoepo.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gtiwtodjzm.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtmgpucvga.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gtbitzsxgq.html

date +%s;  date -d @1700000000
来源：http://hz.snrcjt.cn/gtvbxajlpx.html

[R71] 日期格式化
来源：http://hz.yongpay.top/gtxdmxsskc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cdnleiting.top/gtunwfdxgm.html

[R72] 等待端口就绪
来源：http://hz.gaohongyu789.top/gtijcopwfn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pengpengdd.cyou/gtjhkxyrwj.html

[R73] 分割大日志
来源：http://hz.zhoulong.xyz/gtjmmdaieh.html

split -l 1000 big.log part_
来源：http://hz.aizwys.cn/gtlqusmtwe.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtfqbxofhc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yonumen.top/gtyuwqxomo.html

[R75] 导出环境变量
来源：http://hz.yangfankeji.com/gtakfsjujx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yonumen.top/gtrvemtnpr.html

[R76] 使用临时文件
来源：http://hz.mhx1999.top/gtyqybhjcb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gttnpxqyis.html

[R77] 读取用户输入
来源：http://hz.svipenyu.cn/gtarpzwzya.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtwmhlozuh.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gtyawxuzeg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtznvebdyw.html

[R79] 解析命令行选项
来源：http://hz.hnxiangtu.top/gtqdcgzfoa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.pengpengdd.cyou/gtjqmqmlia.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtzjiudxxl.html

time ./run.sh
来源：http://hz.sufxvd.cn/gtoqnlvvyu.html

================================================================================
来源：http://hz.zhixingplan.top/gtmssqmvfx.html

S. C / C++ 专题
来源：http://hz.mhx1999.top/gtslwguugw.html

================================================================================
来源：http://hz.snrcjt.cn/gtmqarmuyx.html

[S01] C：Hello World
来源：http://hz.shanyushiyangtech.top/gtvandrini.html

#include <stdio.h>
来源：http://hz.ydzc1.top/gtvmmvoobb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.kuanghao11.cn/gtcrkkonil.html

[S02] C：变量与格式化输出
来源：http://hz.fengsongda.top/gtzrwuthug.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gttwemwwri.html

[S03] C：读入整数
来源：http://hz.nanxinkj.top/gtuotyahzj.html

int x; scanf("%d", &x);
来源：http://hz.zhixingplan.top/gtmsllfnqt.html

[S04] C：字符串复制
来源：http://hz.jlsjyb.cn/gtnqgmbman.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtdjicgdud.html

[S05] C：字符串长度
来源：http://hz.hywenlv.cn/gtnrmbcfeo.html

strlen(s)
来源：http://hz.jqgufenzy.top/gtktpwmjnl.html

[S06] C：字符串比较
来源：http://hz.sxryk.cn/gtfgygvxbo.html

strcmp(a, b) == 0
来源：http://hz.cqqwz.cn/gtkntqmlrj.html

[S07] C：数组遍历求和
来源：http://hz.meibo888.top/gtyhskhymq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.meibo888.top/gtsafogcyh.html

[S08] C：动态内存分配与释放
来源：http://hz.jinqigufen.top/gtnmkuqorq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuxming.cn/gtqtdfobdk.html

[S09] C：结构体定义与初始化
来源：http://hz.zhengqikj.top/gtpqwquirz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhongyouzk.top/gtsdusjarl.html

[S10] C：指针与解引用
来源：http://hz.ppjwa.cn/gtmdramfxt.html

int *p = &a;  *p = 5;
来源：http://hz.pycfn.com/gtwwccozvu.html

[S11] C：逐行读文件
来源：http://hz.hnqzz.top/gtmtyfsdsw.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zhoulong.xyz/gthtcunbow.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nanxuanxn.top/gtgxgzdopu.html

fclose(f);
来源：http://hz.shanyushiyangkeji.top/gtwefrosjp.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtkxvwcebf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.xingfuxueyuan.xyz/gtxyneolkq.html

[S13] C：宏定义
来源：http://hz.zhiwuduotai.top/gtinfusucn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yueranfly.top/gtvvqirgal.html

[S14] C：枚举
来源：http://hz.xziqi.cn/gtixkbzcbe.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.guowangkeji.top/gthzoogkyl.html

[S15] C：类型转换
来源：http://hz.sxryk.cn/gtkamxyyqg.html

(double) a / b
来源：http://hz.yongpay.top/gtkxopppxi.html

[S16] C：位操作置位
来源：http://hz.tanke756.top/gtljjkfnku.html

x |= (1 << 3);
来源：http://hz.wangdashe.top/gtuaznlrmc.html

[S17] C：安全拼接字符串
来源：http://hz.ivvv.top/gtgqdyahma.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jqgfzy.top/gtrgnwwial.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtymojwhhi.html

int main(int argc, char **argv)
来源：http://hz.nanxuanxn.top/gtthdusunr.html

[S19] C：快速排序
来源：http://hz.nanxinkj.top/gtpyxujchj.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtnacnfghn.html

[S20] C：二分查找
来源：http://hz.shuidangran.top/gthyvhjhru.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtnlxvqmgs.html

[S21] C：字符类别判断
来源：http://hz.dianchejie.cn/gthtbucgrv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtczxyzdai.html

[S22] C：字符串转数字
来源：http://hz.pycfn.com/gtqpnllbnn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ppjwa.cn/gtvmofmcae.html

[S23] C：随机数
来源：http://hz.hfpthk.cn/gtivxjjwaq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.shangyingyoupin.top/gtzdhafaqv.html

[S24] C：获取本地时间
来源：http://hz.dashuyun.cn/gtzzpogfmg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ydjk.org.cn/gtafnfzknk.html

[S25] C：内存拷贝
来源：http://hz.zhengqikj.top/gtlnvokiox.html

memcpy(dst, src, n);
来源：http://hz.nwbrower.top/gtvkyxbpyy.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtvmizwyuu.html

memset(a, 0, sizeof a);
来源：http://hz.hnxiangtu.top/gtnjrnjqad.html

[S27] C：定义常量
来源：http://hz.jqgufenzy.top/gtcgzghgid.html

const double PI = 3.14159;
来源：http://hz.yuanzhike.top/gtgwmiegam.html

[S28] C：静态变量
来源：http://hz.9152youxi.cn/gtyylquovw.html

static int counter = 0;
来源：http://hz.jinghuilouyu.cn/gtdstkyowu.html

[S29] C：变参函数
来源：http://hz.chenzaomai.com/gthehdtogo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangkeji.top/gtaksjmyrg.html

[S30] C：头文件保护
来源：http://hz.svipenyu.cn/gtfvuxgptc.html

#ifndef X_H
来源：http://hz.chenzaomai.com/gthzyuotif.html

#define X_H
来源：http://hz.bjfxy.top/gtnhojqqji.html

#endif
来源：http://hz.redwolf501.top/gthadinrwn.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtpvfyceje.html

#include <iostream>
来源：http://hz.yangfankeji.com/gtcnyzytaa.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gtlmxhtpei.html

[S32] C++：字符串
来源：http://hz.316326.xyz/gtzctkgjcq.html

std::string s = "hi";  s += "!";
来源：http://hz.shuidangran.top/gtvzvsxesx.html

[S33] C++：vector 增删
来源：http://hz.ppjwa.cn/gthkrakmtd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.wangshuangyany.cn/gtyjccnvwd.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtffapvvrt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yonumen.top/gtfyylmywe.html

[S35] C++：map
来源：http://hz.shangyingyoupin.top/gteozdzbtq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhiwuduotai.top/gtjaimimpj.html

[S36] C++：unordered_map
来源：http://hz.chenlongwang.top/gtgqzpyaun.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cheryme.top/gtlfvzawmj.html

[S37] C++：set
来源：http://hz.316326.xyz/gtwtudjsks.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.nanxuanxn.top/gtzbyaazqk.html

[S38] C++：排序
来源：http://hz.chenjidiqi.icu/gtzpzhhaqy.html

std::sort(v.begin(), v.end());
来源：http://hz.ybcxt.top/gtkkhkakai.html

[S39] C++：自定义比较器排序
来源：http://hz.gzhubu.top/gthjncgpoh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.0kj1m.cn/gtjdqrccwl.html

[S40] C++：查找元素
来源：http://hz.ppjwa.cn/gtyoftnatc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yuxming.cn/gtswolftdf.html

[S41] C++：类与构造函数
来源：http://hz.daxiang520.top/gturaoclyg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gtxjhcbtby.html

[S42] C++：继承与虚函数
来源：http://hz.guowangkeji.top/gtqjsmxcnt.html

class B : public Base { public: void f() override {} };
来源：http://hz.tian-w.cn/gtifdfihmq.html

[S43] C++：智能指针
来源：http://hz.hnqzz.top/gtrjngixfs.html

auto p = std::make_unique<int>(5);
来源：http://hz.nwbrower.top/gtdmihfiyi.html

[S44] C++：引用传参
来源：http://hz.jinyuanbaomall.cn/gtlpigakkn.html

void inc(int &x) { ++x; }
来源：http://hz.chenzaomai.com/gtpqniyhyd.html

[S45] C++：lambda
来源：http://hz.daxiang520.top/gtilvchclr.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.sxryk.cn/gtvdrdkhvw.html

[S46] C++：函数模板
来源：http://hz.smart0.xyz/gtfwulluxh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.daxiang520.top/gtadthkbxs.html

[S47] C++：结构化绑定遍历
来源：http://hz.bjfxy.top/gtxadrboxa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yuxming.cn/gtsqyrizih.html

[S48] C++：逐行读文件
来源：http://hz.cucudq.cn/gtkqxbvthx.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gteutdmpqe.html

while (std::getline(in, line)) { }
来源：http://hz.cdnleiting.top/gtjnqaxgxx.html

[S49] C++：写文件
来源：http://hz.bjfxy.top/gtgwiqpwfu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.jinyuanbaomall.cn/gtvioylqto.html

[S50] C++：格式化数字
来源：http://hz.hnxiangtu.top/gtgzyrgfwf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.iojbl.cn/gtynjguxfk.html

[S51] C++：显式类型转换
来源：http://hz.shuidangran.top/gttkqqdjkv.html

static_cast<double>(a) / b
来源：http://hz.0kj1m.cn/gtrgclrtig.html

[S52] C++：const 与 noexcept
来源：http://hz.ybcxt.top/gtiyvmhwbr.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtdksyelms.html

[S53] C++：移动语义
来源：http://hz.xziqi.cn/gtzuwoxxyy.html

std::vector<int> w = std::move(v);
来源：http://hz.feifeiyinyue.top/gtlrbbwioy.html

[S54] C++：异常处理
来源：http://hz.gotoacloud.top/gtezidvjwb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnxiangtu.top/gtfuposoot.html

[S55] C++：结构化绑定
来源：http://hz.jinqigufen.top/gtaprcqypt.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj20258.top/gtsokbgnua.html

[S56] C++：optional
来源：http://hz.birdmap.top/gtevhjpnun.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jiagoushi.top/gtmqhwhmud.html

[S57] C++：编译期常量
来源：http://hz.xuetiantiany.cn/gtqoyjvruw.html

constexpr int N = 10;
来源：http://hz.shuidangran.top/gtxjmxyndy.html

[S58] C++：命名空间
来源：http://hz.havefunace.top/gtfzlckpbe.html

namespace ns { int f() { return 1; } }
来源：http://hz.aibaodan.cn/gtvdmnjbqp.html

[S59] C++：静态断言
来源：http://hz.hnxiangtu.top/gtzkeixmfa.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zycfv.cn/gtwtnmfqtx.html

[S60] C++：遍历并删除元素
来源：http://hz.yj20258888.top/gthpxumkxm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinyuanbaomall.cn/gtrszlnlpk.html

================================================================================
来源：http://hz.chenzaomai.com/gturjpregs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.smart0.xyz/gtmzjvvsjs.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtlpgscrvv.html

[T01] Kotlin：Hello World
来源：http://hz.9152youxi.cn/gtrljlakdk.html

println("Hello")
来源：http://hz.shzxlz.cn/gtqevlqvur.html

[T02] Kotlin：变量
来源：http://hz.smart0.xyz/gtjfzttdhg.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sxryk.cn/gtpvhblgjc.html

[T03] Kotlin：字符串模板
来源：http://hz.jyoumei.cn/gtgovjlfwt.html

"值: $b"
来源：http://hz.zhoulong.xyz/gteafwsfrs.html

[T04] Kotlin：空安全
来源：http://hz.xingfuxueyuan.xyz/gtvmrafyfa.html

val n: String? = null;  n?.length
来源：http://hz.quarkkingdee.top/gtcnkgjcoi.html

[T05] Kotlin：when 表达式
来源：http://hz.shzxlz.cn/gtfboogojc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.gogol.net.cn/gtdnvrsfuf.html

[T06] Kotlin：集合映射
来源：http://hz.nanxinkj.top/gtjholjebi.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gaohongyu789.top/gttbyqrbjn.html

[T07] Kotlin：集合过滤
来源：http://hz.jyoumei.cn/gtgipapdai.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.redwolf501.top/gtfntasnra.html

[T08] Kotlin：数据类
来源：http://hz.shangyingyoupin.top/gtfrfqhgrk.html

data class User(val name: String, val age: Int)
来源：http://hz.yj202588.top/gtegmlwgzm.html

[T09] Kotlin：扩展函数
来源：http://hz.guowangkeji.top/gtgqjhwwgh.html

fun String.exclaim() = this + "!"
来源：http://hz.chenzaomai.com/gtzrsogucp.html

[T10] Kotlin：默认参数
来源：http://hz.sweek.top/gtzvjmrszs.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gteghrjsho.html

[T11] Kotlin：协程
来源：http://hz.jinghuilouyu.cn/gtgpmtchbu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenjidiqi.icu/gtmkaunbnm.html

[T12] Kotlin：解构声明
来源：http://hz.gotoacloud.top/gtwxvcwoyn.html

val (a, b) = Pair(1, 2)
来源：http://hz.fzhhl.top/gtqkbytwoz.html

[T13] Kotlin：只读 Map
来源：http://hz.tianlin.xyz/gtifmpktal.html

val m = mapOf("a" to 1)
来源：http://hz.fzhhl.top/gtbfcodzmu.html

[T14] Kotlin：循环
来源：http://hz.gotoacloud.top/gtazthxhaq.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtiilxgubm.html

[T15] Kotlin：接口
来源：http://hz.wangdashe.top/gtiepvbspt.html

interface Shape { fun area(): Double }
来源：http://hz.fzhhl.top/gtvtwfrylv.html

[T16] Swift：Hello World
来源：http://hz.zhixingplan.top/gtgquwhdlt.html

print("Hello")
来源：http://hz.wangdashe.top/gtmstcmosw.html

[T17] Swift：变量与常量
来源：http://hz.fengsongda.top/gtvaocdrct.html

var a = 1;  let b = 2
来源：http://hz.hnqzz.top/gtysmkhqau.html

[T18] Swift：字符串插值
来源：http://hz.fengsongda.top/gtliotppfm.html

"值: \(b)"
来源：http://hz.zhijiandao.cn/gthyjnxade.html

[T19] Swift：可选绑定
来源：http://hz.cdnleiting.top/gtdxxijasx.html

if let n = opt { print(n) }
来源：http://hz.hfpthk.cn/gtexglqsgo.html

[T20] Swift：数组操作
来源：http://hz.xingfuxueyuan.xyz/gtfilfmilj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.yvedp.cn/gtwmbcudzw.html

[T21] Swift：遍历
来源：http://hz.zhaomingkeji.xyz/gtjtyjrrqc.html

for x in a { print(x) }
来源：http://hz.jinqigufen.top/gtkemleuru.html

[T22] Swift：字典
来源：http://hz.chenzaomai.com/gtqqpoudmg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.sysykeji.top/gtwtigdlas.html

[T23] Swift：函数
来源：http://hz.aizwys.cn/gtbaqyzyul.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xylfe.cn/gtbkdjypnp.html

[T24] Swift：闭包
来源：http://hz.svipenyu.cn/gtafmvsqaq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.snrcjt.cn/gtdxwibsgx.html

[T25] Swift：结构体
来源：http://hz.daria6918.cn/gtiwzttzph.html

struct P { var x: Int }
来源：http://hz.cucudq.cn/gtqseastal.html

[T26] Swift：类与重写
来源：http://hz.yj20258888.top/gtwrocszdm.html

class A: Base { override func f() {} }
来源：http://hz.yanxiufei.cn/gtyrlbrzwu.html

[T27] Swift：错误处理
来源：http://hz.gaohongyu789.top/gttvvawofh.html

do { try f() } catch { print(error) }
来源：http://hz.andypj.xyz/gttwutzden.html

[T28] Swift：枚举
来源：http://hz.meibo888.top/gtgoacwlel.html

enum Color { case red, green }
来源：http://hz.yanxiufei.cn/gtrzijpmzi.html

[T29] Swift：guard 提前返回
来源：http://hz.cucudq.cn/gtswrlnwiv.html

guard let x = opt else { return }
来源：http://hz.wangshuangyany.cn/gtzdrokvdu.html

[T30] Swift：协议
来源：http://hz.haohaochexian.top/gtrydzqalk.html

protocol Shape { func area() -> Double }
来源：http://hz.ybcxt.top/gtuwhdiice.html

[T31] Lua：Hello World
来源：http://hz.meibo888.top/gtxxuttnqm.html

print("Hello")
来源：http://hz.zhaomingkeji.xyz/gtkjlglkkh.html

[T32] Lua：局部变量
来源：http://hz.zhijiandao.cn/gtawezlkwz.html

local a = 1
来源：http://hz.sxryk.cn/gtcqvywblf.html

[T33] Lua：表（数组）
来源：http://hz.mhx1999.top/gtgfizckdj.html

local t = {1, 2, 3};  t[4] = 4
来源：http://hz.nwbrower.top/gtngleevwn.html

[T34] Lua：遍历表
来源：http://hz.hammf.cn/gtofkizznt.html

for i, v in ipairs(t) do print(i, v) end
来源：http://hz.xziqi.cn/gtjbnauwid.html


<!-- 参考信息 -->