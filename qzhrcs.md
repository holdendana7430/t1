代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtrkipebju.html

[R30] 函数返回状态码
来源：http://hz.hnqzz.top/gtiicnjtcc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cucudq.cn/gtjkfdvlmb.html

[R31] 局部变量
来源：http://hz.daxiang520.top/gthzbrahdf.html

f() { local x=1; echo "$x"; }
来源：http://hz.zycfv.cn/gtdsaacwbk.html

[R32] 参数个数校验
来源：http://hz.jinyuanbaomall.cn/gtjazidtww.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtgbkedfan.html

[R33] 捕获错误并提示行号
来源：http://hz.gotoacloud.top/gtlefjbsnv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.gaohongyu789.top/gtmspgrwnt.html

[R34] 退出时清理
来源：http://hz.hfpthk.cn/gtawlskgfn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pengpengdd.cyou/gtmbfztuzw.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtfxhlxidi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gogol.net.cn/gtktrrgnao.html

[R36] 并发执行多个任务
来源：http://hz.wangdashe.top/gtnzaqvsse.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.wangdashe.top/gtgdcmhqbe.html

[R37] 把输出赋给变量
来源：http://hz.yuxming.cn/gtylivhdcp.html

files=$(ls -1)
来源：http://hz.jqgfzy.top/gtmmrbfpah.html

[R38] 管道串联
来源：http://hz.nanxinkj.top/gtsdcldhmv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuetiantiany.cn/gtroajgfky.html

[R39] 重定向标准输出与错误
来源：http://hz.ppjwa.cn/gtraopzlrg.html

cmd > out.log 2>&1
来源：http://hz.iojbl.cn/gtivnnacnc.html

[R40] 追加写日志
来源：http://hz.zhixingplan.top/gthzgupwaa.html

echo "log" >> out.log
来源：http://hz.gogol.net.cn/gtgxmufebp.html

[R41] 丢弃输出
来源：http://hz.52xcode.cn/gttlbbgzye.html

cmd >/dev/null 2>&1
来源：http://hz.birdmap.top/gtaarxoxtv.html

[R42] 输入重定向
来源：http://hz.pycfn.com/gtlznlfpcs.html

wc -l < a.txt
来源：http://hz.fengsongda.top/gtrdujplye.html

[R43] 按名字查找文件
来源：http://hz.yuxming.cn/gtnclvoniv.html

find . -name "*.log" -type f
来源：http://hz.pycfn.com/gtxnodlybw.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gtigndqmph.html

find . -mtime -7 -type f
来源：http://hz.jiagoushi.top/gtppqckaec.html

[R45] 批量删除
来源：http://hz.sxryk.cn/gtlyrtiioa.html

find . -name "*.tmp" -delete
来源：http://hz.zhixingplan.top/gtqsfilxuy.html

[R46] 递归替换文件内容
来源：http://hz.vqdsnc.cn/gthdnugusp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigfzy.top/gttylweqty.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtwhinwuql.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.dashuyun.cn/gtqbwrufrj.html

[R48] awk 取指定列
来源：http://hz.gaohongyu789.top/gtwkfjsniq.html

awk '{print $1, $3}' a.txt
来源：http://hz.yj20258888.top/gtinbgcdui.html

[R49] awk 带条件
来源：http://hz.birdmap.top/gtfifmmhci.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.snrcjt.cn/gtlslcvnkj.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtnfbgsmjm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.gzhubu.top/gtcigazbwf.html

[R51] 排序去重取前几
来源：http://hz.xuanzx.com/gtlcuuvzgh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yj202588.top/gtdyyqfoep.html

[R52] 统计行数
来源：http://hz.wangdashe.top/gtqxvyydps.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtmtttroax.html

[R53] 查看文件头与实时尾
来源：http://hz.yj202588.top/gtmmxrmnio.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gtwzpkvnun.html

[R54] 比较两个文件
来源：http://hz.guowangkeji.top/gtzhpgxaxm.html

diff a.txt b.txt
来源：http://hz.xinyue.icu/gtinmgaihk.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtmjddutjj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gtgsvmlbum.html

[R56] 远程拷贝
来源：http://hz.birdmap.top/gtviafxsux.html

scp file user@host:/path/
来源：http://hz.gzhubu.top/gtejsmntjc.html

[R57] 远程执行命令
来源：http://hz.yuxming.cn/gtbxfrhatu.html

ssh user@host 'uptime'
来源：http://hz.guannengcc.top/gtblmicjxe.html

[R58] 下载文件
来源：http://hz.yonumen.top/gtxwlodfww.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cucudq.cn/gtoqxmfghi.html

[R59] 发 POST JSON
来源：http://hz.hongshengwenyu.top/gtzignjlfh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.mhx1999.top/gtooakywoh.html

[R60] 只看 HTTP 状态码
来源：http://hz.sufxvd.cn/gtqsogvejq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtfogkuanb.html

[R61] 磁盘占用
来源：http://hz.zhongyouzk.top/gtmxbldegk.html

df -h;  du -sh *
来源：http://hz.shangyingyoupin.top/gtbazmyafv.html

[R62] 找最占空间的文件
来源：http://hz.0kj1m.cn/gtecoeyvjk.html

du -ah . | sort -rh | head -10
来源：http://hz.tianlin.xyz/gtmetqriau.html

[R63] 内存与进程
来源：http://hz.yangfankeji.com/gtbuzdmpvd.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtmaicwxhi.html

[R64] 结束进程
来源：http://hz.jinqigufen.top/gtbnsfpyos.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xziqi.cn/gtjrozhyeo.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtikomilej.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.ivvv.top/gtquvaygrr.html

[R66] 定时任务
来源：http://hz.hywenlv.cn/gtumcmvxuh.html

crontab -e;  crontab -l
来源：http://hz.cheryme.top/gtecujwucu.html

[R67] 生成随机十六进制串
来源：http://hz.xingfuxueyuan.xyz/gtdzpwarif.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtjhknyjyy.html

[R68] 计算文件校验值
来源：http://hz.zhoulong.xyz/gtrpmfueie.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhijiandao.cn/gtlewirxiu.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtpkrunsww.html

head -c 16 /dev/urandom | base64
来源：http://hz.yangfankeji.com/gtjujltgmw.html

[R70] 时间戳与互转
来源：http://hz.ydjk.org.cn/gtvjbqvffo.html

date +%s;  date -d @1700000000
来源：http://hz.pengpengdd.cyou/gtcpazexzp.html

[R71] 日期格式化
来源：http://hz.birdmap.top/gttczruoit.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daxiang520.top/gtzkzhjepy.html

[R72] 等待端口就绪
来源：http://hz.snrcjt.cn/gtqvauqlug.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yvedp.cn/gtanwcaecc.html

[R73] 分割大日志
来源：http://hz.xziqi.cn/gtrsnldppi.html

split -l 1000 big.log part_
来源：http://hz.zdqjudy.top/gtqwayensh.html

[R74] 批量重命名
来源：http://hz.gotoacloud.top/gtuzzplqte.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.ehwqpu.com/gtfuzejrwn.html

[R75] 导出环境变量
来源：http://hz.chenlongwang.top/gtztixsbgs.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.daria6918.cn/gtxafyxmbz.html

[R76] 使用临时文件
来源：http://hz.jqgufenzy.top/gtcpdcesix.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtewqoaodh.html

[R77] 读取用户输入
来源：http://hz.cdnleiting.top/gtqvxipsrb.html

read -rp "请输入: " ans
来源：http://hz.yvedp.cn/gtrraxxvhj.html

[R78] 交互式菜单
来源：http://hz.havefunace.top/gtajbdsbnl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dianchejie.cn/gtvtmmhpph.html

[R79] 解析命令行选项
来源：http://hz.mhx1999.top/gtmhzzskio.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.guowangkeji.top/gtvwitvivn.html

[R80] 查看脚本执行耗时
来源：http://hz.guowangkeji.top/gtxwrqpfgw.html

time ./run.sh
来源：http://hz.hywenlv.cn/gtkpperrnl.html

================================================================================
来源：http://hz.jyoumei.cn/gthabwbont.html

S. C / C++ 专题
来源：http://hz.dianchejie.cn/gtbrwykrwu.html

================================================================================
来源：http://hz.cucudq.cn/gtteggatli.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtnmmhfowc.html

#include <stdio.h>
来源：http://hz.zhixingplan.top/gtqvzchlhg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.haohaochexian.top/gtlpmhqmum.html

[S02] C：变量与格式化输出
来源：http://hz.shanyushiyangtech.top/gtuxfqdxhd.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gtogwczrwk.html

[S03] C：读入整数
来源：http://hz.hfpthk.cn/gtkjgfmxzs.html

int x; scanf("%d", &x);
来源：http://hz.jqgufenzy.top/gtnjbhniun.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gtosfnjtfp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtfqxkfgkb.html

[S05] C：字符串长度
来源：http://hz.jyoumei.cn/gtikacrbfu.html

strlen(s)
来源：http://hz.0kj1m.cn/gtuhcknhbc.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtzrzbockx.html

strcmp(a, b) == 0
来源：http://hz.yj20258888.top/gtabvimcuz.html

[S07] C：数组遍历求和
来源：http://hz.aibaodan.cn/gtprrcqmrr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.shanyushiyangtech.top/gtchfbduwv.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtewrrlwuu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.gotoacloud.top/gtnaxybbta.html

[S09] C：结构体定义与初始化
来源：http://hz.sweek.top/gtqzesnrgv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gthkkkqkez.html

[S10] C：指针与解引用
来源：http://hz.jinqigufen.top/gtkgopchfp.html

int *p = &a;  *p = 5;
来源：http://hz.hnxiangtu.top/gtsautvvrv.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtmetexssx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtylpljcol.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shzxlz.cn/gtpcwfzbul.html

fclose(f);
来源：http://hz.yonumen.top/gtzrqomxnw.html

[S12] C：写文件
来源：http://hz.yvedp.cn/gtbiojnzns.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.daxiang520.top/gtcwlzdyja.html

[S13] C：宏定义
来源：http://hz.tian-w.cn/gtsvpjdcfn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.0kj1m.cn/gtuekmgnrl.html

[S14] C：枚举
来源：http://hz.chenlongwang.top/gtzfgtwlna.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhaomingkeji.xyz/gtffhitahb.html

[S15] C：类型转换
来源：http://hz.tian-w.cn/gtvjlsxqvq.html

(double) a / b
来源：http://hz.yj20258.top/gtczgxsflz.html

[S16] C：位操作置位
来源：http://hz.jinyuanbaomall.cn/gtnyjjnprn.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gtshbtuung.html

[S17] C：安全拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtamfexvzg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtekyqluzh.html

[S18] C：命令行参数
来源：http://hz.ehwqpu.com/gtlmxohspp.html

int main(int argc, char **argv)
来源：http://hz.smart0.xyz/gtbltwopiy.html

[S19] C：快速排序
来源：http://hz.cqqwz.cn/gtgithuqxz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ydjk.org.cn/gtvqvabffm.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtbrfvfghr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.tanke756.top/gtsgaxhzoz.html

[S21] C：字符类别判断
来源：http://hz.0kj1m.cn/gtkfqdetbk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuetiantiany.cn/gtvudeifgx.html

[S22] C：字符串转数字
来源：http://hz.zhiwuduotai.top/gtquhrgrsj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cucudq.cn/gtnucpncqj.html

[S23] C：随机数
来源：http://hz.zhaomingkeji.xyz/gtgcebdxep.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yanxiufei.cn/gtdmmuklyv.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtvmaeuqsw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuanzhike.top/gtpwmnqsqh.html

[S25] C：内存拷贝
来源：http://hz.jlsjyb.cn/gtjfvjobhc.html

memcpy(dst, src, n);
来源：http://hz.shangyingyoupin.top/gtejxhcfkw.html

[S26] C：内存清零
来源：http://hz.nanxuanxn.top/gtzqvpecpd.html

memset(a, 0, sizeof a);
来源：http://hz.sysykeji.top/gtybgycjgn.html

[S27] C：定义常量
来源：http://hz.hywenlv.cn/gtjlzmjfzr.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtspoocfrv.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtbqyakxmn.html

static int counter = 0;
来源：http://hz.jinqigfzy.top/gtznjhryff.html

[S29] C：变参函数
来源：http://hz.tian-w.cn/gtrimbeqln.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtmfddqwgr.html

[S30] C：头文件保护
来源：http://hz.ydzc1.top/gtdfcfttyq.html

#ifndef X_H
来源：http://hz.zycfv.cn/gtvtxmujsl.html

#define X_H
来源：http://hz.ehwqpu.com/gtxcpucogq.html

#endif
来源：http://hz.guannengcc.top/gtuofzlzgp.html

[S31] C++：Hello World
来源：http://hz.vqdsnc.cn/gtkadgkkkm.html

#include <iostream>
来源：http://hz.pycfn.com/gtbsozwhgw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtoxkimzpd.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtatqyzkuj.html

std::string s = "hi";  s += "!";
来源：http://hz.dashuyun.cn/gtuvcmgbhm.html

[S33] C++：vector 增删
来源：http://hz.zhiwuduotai.top/gtzcwmblpu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cashguo.top/gtabeudcnz.html

[S34] C++：遍历 vector
来源：http://hz.hammf.cn/gtdigdgiwd.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.hongshengwenyu.top/gtplqztrxf.html

[S35] C++：map
来源：http://hz.redwolf501.top/gtfsszcbhs.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gtsqccsipk.html

[S36] C++：unordered_map
来源：http://hz.gaohongyu789.top/gthuzgggaq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtdntodrpe.html

[S37] C++：set
来源：http://hz.redwolf501.top/gtnlgzinlu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tianlin.xyz/gtssdbltej.html

[S38] C++：排序
来源：http://hz.xinyue.icu/gtviexxdeo.html

std::sort(v.begin(), v.end());
来源：http://hz.yj202588.top/gtqpjweokp.html

[S39] C++：自定义比较器排序
来源：http://hz.zhoulong.xyz/gtagjuoeri.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jqgfzy.top/gtdkxpqdes.html

[S40] C++：查找元素
来源：http://hz.zhixingplan.top/gtovcjrdmz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtcttarjfb.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtnzsqpgzo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.guannengcc.top/gtzbxpwbnn.html

[S42] C++：继承与虚函数
来源：http://hz.gogol.net.cn/gtnhyrxomn.html

class B : public Base { public: void f() override {} };
来源：http://hz.shuidangran.top/gtnukpquef.html

[S43] C++：智能指针
来源：http://hz.xingfuxueyuan.xyz/gtpwohnxjf.html

auto p = std::make_unique<int>(5);
来源：http://hz.guannengcc.top/gtmzslgosn.html

[S44] C++：引用传参
来源：http://hz.havefunace.top/gtelitazuu.html

void inc(int &x) { ++x; }
来源：http://hz.svipenyu.cn/gtqvdezzai.html

[S45] C++：lambda
来源：http://hz.yj20258888.top/gtilsxhpxl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hywenlv.cn/gtiktuybfx.html

[S46] C++：函数模板
来源：http://hz.sufxvd.cn/gteqftdnte.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hfpthk.cn/gtorjwkqxc.html

[S47] C++：结构化绑定遍历
来源：http://hz.quarkkingdee.top/gtsyjgocby.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gttuynoujb.html

[S48] C++：逐行读文件
来源：http://hz.jinqigufen.top/gtnwwttngo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtxkbugumy.html

while (std::getline(in, line)) { }
来源：http://hz.haohaochexian.top/gtjqscnjet.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gtsuyuykct.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.havefunace.top/gtyroirqea.html

[S50] C++：格式化数字
来源：http://hz.yongpay.top/gthbntmykk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hfpthk.cn/gtcwjrbeds.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gtxcsdactq.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtgrjaxshp.html

[S52] C++：const 与 noexcept
来源：http://hz.ppjwa.cn/gtumwkjusr.html

int size() const noexcept { return n_; }
来源：http://hz.hnqzz.top/gtflqzqsbt.html

[S53] C++：移动语义
来源：http://hz.jiagoushi.top/gtyukobrdz.html

std::vector<int> w = std::move(v);
来源：http://hz.cqqwz.cn/gtkqzknpvo.html

[S54] C++：异常处理
来源：http://hz.c1oappe.top/gthyfffgio.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jyoumei.cn/gtdoliqnmt.html

[S55] C++：结构化绑定
来源：http://hz.shangyingyoupin.top/gtpplturvf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhongyouzk.top/gtkuehahlv.html

[S56] C++：optional
来源：http://hz.vqdsnc.cn/gtytncrdlz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.wangdashe.top/gtfmptwhqo.html

[S57] C++：编译期常量
来源：http://hz.yj202588.top/gtgyuwdnwk.html

constexpr int N = 10;
来源：http://hz.hywenlv.cn/gtctkgozgx.html

[S58] C++：命名空间
来源：http://hz.cashguo.top/gttrgpvadr.html

namespace ns { int f() { return 1; } }
来源：http://hz.sxryk.cn/gtpqkrskid.html

[S59] C++：静态断言
来源：http://hz.fzhhl.top/gtlrckjafr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.guowangkeji.top/gtazcjnwlx.html

[S60] C++：遍历并删除元素
来源：http://hz.zhiwuduotai.top/gthisgnwms.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtnuhdsjbx.html

================================================================================
来源：http://hz.gotoacloud.top/gtcqcgrefc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jqgfzy.top/gtfgbxaqgm.html

================================================================================
来源：http://hz.chenjidiqi.icu/gteurmydiv.html

[T01] Kotlin：Hello World
来源：http://hz.yj20258.top/gtkssqkhbn.html

println("Hello")
来源：http://hz.xingfuxueyuan.xyz/gtufqvsmsw.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gtvoudueiq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtenmmeiqn.html

[T03] Kotlin：字符串模板
来源：http://hz.jiagoushi.top/gtfuhkmfrg.html

"值: $b"
来源：http://hz.daxiang520.top/gtifywtrzs.html

[T04] Kotlin：空安全
来源：http://hz.cashguo.top/gtzmvbzcxd.html

val n: String? = null;  n?.length
来源：http://hz.sweek.top/gtlfoqlcwj.html

[T05] Kotlin：when 表达式
来源：http://hz.zhaomingkeji.xyz/gtlfzcqgkm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.guannengcc.top/gtxasfdldz.html

[T06] Kotlin：集合映射
来源：http://hz.chenzaomai.com/gtgdnzrxmv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.svipenyu.cn/gtxarhmfwp.html

[T07] Kotlin：集合过滤
来源：http://hz.jinghuilouyu.cn/gtuzcbvgey.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yvedp.cn/gtumigfoom.html

[T08] Kotlin：数据类
来源：http://hz.gotoacloud.top/gtasxpiyra.html

data class User(val name: String, val age: Int)
来源：http://hz.quarkkingdee.top/gtleacmavr.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtvhwyjygw.html

fun String.exclaim() = this + "!"
来源：http://hz.nwbrower.top/gtqoquqfqh.html

[T10] Kotlin：默认参数
来源：http://hz.jinghuilouyu.cn/gtfhupwwds.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtiolwbiul.html

[T11] Kotlin：协程
来源：http://hz.xuetiantiany.cn/gtrfemuzax.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.xinyue.icu/gteuyzuinv.html

[T12] Kotlin：解构声明
来源：http://hz.jinghuilouyu.cn/gtvwxumkpn.html

val (a, b) = Pair(1, 2)
来源：http://hz.yj20258.top/gtddayjhsd.html

[T13] Kotlin：只读 Map
来源：http://hz.quarkkingdee.top/gteanwjfmo.html

val m = mapOf("a" to 1)
来源：http://hz.hysaishi.cn/gtpbaffxwa.html

[T14] Kotlin：循环
来源：http://hz.yangfankeji.com/gteakvummp.html

for (i in 1..10) println(i)
来源：http://hz.xinyue.icu/gttablgbov.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gtpboogmwr.html

interface Shape { fun area(): Double }
来源：http://hz.hongshengwenyu.top/gtcjtalhuj.html

[T16] Swift：Hello World
来源：http://hz.nanxuanxn.top/gtrtxjvpxs.html

print("Hello")
来源：http://hz.cheryme.top/gtpmkdunuw.html

[T17] Swift：变量与常量
来源：http://hz.dashuyun.cn/gttkzkfkhs.html

var a = 1;  let b = 2
来源：http://hz.hywenlv.cn/gterxrcadn.html

[T18] Swift：字符串插值
来源：http://hz.shanyushiyangtech.top/gtytpwolqe.html

"值: \(b)"
来源：http://hz.ydjk.org.cn/gtlllxehjj.html

[T19] Swift：可选绑定
来源：http://hz.ybcxt.top/gttzyvhdpp.html

if let n = opt { print(n) }
来源：http://hz.yj202588.top/gtyctutqea.html

[T20] Swift：数组操作
来源：http://hz.jinyuanbaomall.cn/gtnarurxqe.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.sweek.top/gtkaeqytzn.html

[T21] Swift：遍历
来源：http://hz.bjfxy.top/gtnbpndtia.html

for x in a { print(x) }
来源：http://hz.gzhubu.top/gtxmgtwhrk.html

[T22] Swift：字典
来源：http://hz.nanxuanxn.top/gtnakwbwyq.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhongyouzk.top/gtrdtrwfbo.html

[T23] Swift：函数
来源：http://hz.zycfv.cn/gtqgsufcjb.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.shuidangran.top/gtyhowhwop.html

[T24] Swift：闭包
来源：http://hz.chenlongwang.top/gtnhqpxfjq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jqgufenzy.top/gtnlthucvg.html

[T25] Swift：结构体
来源：http://hz.wangdashe.top/gtobfkjivj.html

struct P { var x: Int }
来源：http://hz.tianlin.xyz/gtsiwpderu.html

[T26] Swift：类与重写
来源：http://hz.hnqzz.top/gtftsocvye.html

class A: Base { override func f() {} }
来源：http://hz.dashuyun.cn/gtoecutosu.html

[T27] Swift：错误处理
来源：http://hz.cheryme.top/gtgylbumhk.html

do { try f() } catch { print(error) }
来源：http://hz.dianchejie.cn/gtxopqzdst.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtvqeyrtus.html

enum Color { case red, green }
来源：http://hz.yonumen.top/gtolnkoxxa.html

[T29] Swift：guard 提前返回
来源：http://hz.haohaochexian.top/gtbzwokpsr.html

guard let x = opt else { return }
来源：http://hz.xingfuxueyuan.xyz/gtgidolpvk.html

[T30] Swift：协议
来源：http://hz.jinghuilouyu.cn/gtblrbvjqt.html

protocol Shape { func area() -> Double }
来源：http://hz.daxiang520.top/gtkkociiqb.html

[T31] Lua：Hello World
来源：http://hz.redwolf501.top/gtnljdawlt.html

print("Hello")
来源：http://hz.ppjwa.cn/gtnkmrmwqe.html

[T32] Lua：局部变量
来源：http://hz.tianlin.xyz/gtecdmsimn.html

local a = 1
来源：http://hz.pengpengdd.cyou/gtjpvzmvsc.html


<!-- 参考信息 -->