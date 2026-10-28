代发 wailian999

echo $((1 + 2 * 3))
来源：http://hz.wangshuangyany.cn/gtqfrzgkss.html

[R28] 浮点运算
来源：http://hz.zdqjudy.top/gtbzjyuzxg.html

echo "scale=2; 10/3" | bc
来源：http://hz.kuanghao11.cn/gtlwiodhub.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gtfapwaybo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.guowangkeji.top/gtvjxzztgm.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gthgljfufl.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yuanzhike.top/gtdaitclcn.html

[R31] 局部变量
来源：http://hz.dashuyun.cn/gtnegxrrbs.html

f() { local x=1; echo "$x"; }
来源：http://hz.tian-w.cn/gtftswrcib.html

[R32] 参数个数校验
来源：http://hz.feifeiyinyue.top/gtdmxmmayq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtgpxcnzik.html

[R33] 捕获错误并提示行号
来源：http://hz.gogol.net.cn/gtcflpikub.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenjidiqi.icu/gtmdmvsoxz.html

[R34] 退出时清理
来源：http://hz.fengsongda.top/gtwqprxlct.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtcwdjcztp.html

[R35] 后台执行并等待
来源：http://hz.ppjwa.cn/gtuvdngvtp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.zhengqikj.top/gtocuavmwy.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtvwgsoute.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sxryk.cn/gtgbfvacrc.html

[R37] 把输出赋给变量
来源：http://hz.fengsongda.top/gtiywgsdix.html

files=$(ls -1)
来源：http://hz.zycfv.cn/gtpyyirmub.html

[R38] 管道串联
来源：http://hz.aibaodan.cn/gtlqzgdpda.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ywan-chungtsiang.top/gtlsvazohv.html

[R39] 重定向标准输出与错误
来源：http://hz.hammf.cn/gtexvlbskp.html

cmd > out.log 2>&1
来源：http://hz.guannengcc.top/gtmdmxrjba.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtseecztqz.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gtgtprqzys.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtbqmqrsii.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gtlqyinzxb.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gthgigwgkr.html

wc -l < a.txt
来源：http://hz.9152youxi.cn/gtqeoiidcr.html

[R43] 按名字查找文件
来源：http://hz.svipenyu.cn/gtrwxtwhzl.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtgklwwvpf.html

[R44] 按修改时间查找
来源：http://hz.yueranfly.top/gtzzngiusl.html

find . -mtime -7 -type f
来源：http://hz.aibaodan.cn/gtdcnwpsnd.html

[R45] 批量删除
来源：http://hz.ivvv.top/gtogbpdkug.html

find . -name "*.tmp" -delete
来源：http://hz.pycfn.com/gtdswvbxwt.html

[R46] 递归替换文件内容
来源：http://hz.pycfn.com/gtnoiedfkq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtilymfghe.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtsikinddz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ppjwa.cn/gtxiemqbpe.html

[R48] awk 取指定列
来源：http://hz.zdqjudy.top/gtewinttsy.html

awk '{print $1, $3}' a.txt
来源：http://hz.daxiang520.top/gtoazdkqsm.html

[R49] awk 带条件
来源：http://hz.sweek.top/gtavbcqsuw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.hnqzz.top/gtcehqbaxv.html

[R50] awk 求和
来源：http://hz.guannengcc.top/gtcoipgwsb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.sweek.top/gtgywrfqwn.html

[R51] 排序去重取前几
来源：http://hz.yj20258.top/gtqlmhyses.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinghuilouyu.cn/gtunfcofve.html

[R52] 统计行数
来源：http://hz.yangfankeji.com/gtbnzszbpt.html

wc -l a.txt
来源：http://hz.sufxvd.cn/gtdojahuxt.html

[R53] 查看文件头与实时尾
来源：http://hz.andypj.xyz/gtkxbuwieg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zhengqikj.top/gtfwelhmcc.html

[R54] 比较两个文件
来源：http://hz.jinqigufen.top/gtmkrswsgj.html

diff a.txt b.txt
来源：http://hz.fengsongda.top/gtmpxsjwgj.html

[R55] 压缩与解压
来源：http://hz.shanyushiyangkeji.top/gtvbpaivgk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtgxkdpydj.html

[R56] 远程拷贝
来源：http://hz.zdqjudy.top/gthrrwgloo.html

scp file user@host:/path/
来源：http://hz.iojbl.cn/gtpveizrpf.html

[R57] 远程执行命令
来源：http://hz.svipenyu.cn/gtowccbmko.html

ssh user@host 'uptime'
来源：http://hz.quarkkingdee.top/gtuetxwzvy.html

[R58] 下载文件
来源：http://hz.sxryk.cn/gteyjrdrzf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cheryme.top/gtvgxeiwrd.html

[R59] 发 POST JSON
来源：http://hz.zhixingplan.top/gtpaymnrjf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtkmalfybf.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gtmeymzgdy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gogol.net.cn/gtyrwmvhdm.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gtzoxmxpie.html

df -h;  du -sh *
来源：http://hz.shuidangran.top/gttftmrlul.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtbvdhceph.html

du -ah . | sort -rh | head -10
来源：http://hz.52xcode.cn/gtlwdptqqt.html

[R63] 内存与进程
来源：http://hz.zycfv.cn/gtfspnsqob.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtergnrdqo.html

[R64] 结束进程
来源：http://hz.jiagoushi.top/gtrhmspovm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gttkciaxvu.html

[R65] 查看端口占用
来源：http://hz.haohaochexian.top/gtohfzqlnp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtwsjtyiou.html

[R66] 定时任务
来源：http://hz.kuanghao11.cn/gtjxufkjwp.html

crontab -e;  crontab -l
来源：http://hz.pycfn.com/gtngkhqqsx.html

[R67] 生成随机十六进制串
来源：http://hz.hywenlv.cn/gtmyattzsy.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gtfmfjibzz.html

[R68] 计算文件校验值
来源：http://hz.zhiwuduotai.top/gtygmnxqbh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtuexfqmng.html

[R69] 生成随机密码
来源：http://hz.hammf.cn/gtrofcmnuo.html

head -c 16 /dev/urandom | base64
来源：http://hz.yuxming.cn/gtjekulihm.html

[R70] 时间戳与互转
来源：http://hz.guowangkeji.top/gtspwnzdwt.html

date +%s;  date -d @1700000000
来源：http://hz.tian-w.cn/gttalzuhcz.html

[R71] 日期格式化
来源：http://hz.gaohongyu789.top/gtjbgdefre.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.daria6918.cn/gterbasohj.html

[R72] 等待端口就绪
来源：http://hz.guowangkeji.top/gtczysuvdf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinqigufen.top/gtpvliridm.html

[R73] 分割大日志
来源：http://hz.ivvv.top/gtfyjepqyb.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtnufvhzyk.html

[R74] 批量重命名
来源：http://hz.jlsjyb.cn/gtquswlumv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.daxiang520.top/gtyytohryl.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtvxqckges.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhijiandao.cn/gtjbofsabn.html

[R76] 使用临时文件
来源：http://hz.haohaochexian.top/gtpsbwmooq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangkeji.top/gtotocmxau.html

[R77] 读取用户输入
来源：http://hz.nanxuanxn.top/gtkwyzamta.html

read -rp "请输入: " ans
来源：http://hz.jinqigufen.top/gtizfqlbvw.html

[R78] 交互式菜单
来源：http://hz.xuetiantiany.cn/gtfjpkmqao.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ivvv.top/gttsyiflsy.html

[R79] 解析命令行选项
来源：http://hz.dianchejie.cn/gtfxiyclqi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuxming.cn/gtnoovhlns.html

[R80] 查看脚本执行耗时
来源：http://hz.cqqwz.cn/gtxlzxiypq.html

time ./run.sh
来源：http://hz.yvedp.cn/gtletsmufq.html

================================================================================
来源：http://hz.zhongyouzk.top/gtrpdewhjr.html

S. C / C++ 专题
来源：http://hz.yangfankeji.com/gtlzbnxvan.html

================================================================================
来源：http://hz.316326.xyz/gtvxsrsbbh.html

[S01] C：Hello World
来源：http://hz.9152youxi.cn/gtyzsevwve.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtciqutqmc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hysaishi.cn/gtagowpgzg.html

[S02] C：变量与格式化输出
来源：http://hz.ywan-chungtsiang.top/gtdmusngel.html

int a = 10; printf("%d\n", a);
来源：http://hz.andypj.xyz/gtlsvhfuwx.html

[S03] C：读入整数
来源：http://hz.zhaomingkeji.xyz/gtbpfkhxqd.html

int x; scanf("%d", &x);
来源：http://hz.svipenyu.cn/gtshekbnsm.html

[S04] C：字符串复制
来源：http://hz.nwbrower.top/gtohetuyhr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cdnleiting.top/gtatltvrou.html

[S05] C：字符串长度
来源：http://hz.tianlin.xyz/gtqmpglndo.html

strlen(s)
来源：http://hz.cheryme.top/gtyyqorlun.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gtembuldqn.html

strcmp(a, b) == 0
来源：http://hz.yvedp.cn/gtamxfdzng.html

[S07] C：数组遍历求和
来源：http://hz.jqgfzy.top/gttibjlwua.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhiwuduotai.top/gtnetxkmbt.html

[S08] C：动态内存分配与释放
来源：http://hz.iojbl.cn/gtpdkubnpc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.9152youxi.cn/gtbeycjrzk.html

[S09] C：结构体定义与初始化
来源：http://hz.zhiwuduotai.top/gtwsallexb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.9152youxi.cn/gttukavwif.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtdrmokadt.html

int *p = &a;  *p = 5;
来源：http://hz.dianchejie.cn/gtekjuotwk.html

[S11] C：逐行读文件
来源：http://hz.ybcxt.top/gtouwjnmbm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtkirzxtly.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.shanyushiyangkeji.top/gtaeofdnna.html

fclose(f);
来源：http://hz.gaohongyu789.top/gttozesabd.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtvbciyavx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.52xcode.cn/gtkdipyxel.html

[S13] C：宏定义
来源：http://hz.jlsjyb.cn/gttpjdgfxp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gtdecdttht.html

[S14] C：枚举
来源：http://hz.wangshuangyany.cn/gtiunozama.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shanyushiyangkeji.top/gtnprcrpbo.html

[S15] C：类型转换
来源：http://hz.zhoulong.xyz/gtzdqajxbk.html

(double) a / b
来源：http://hz.guowangkeji.top/gtfivxmijj.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtjsrofdjv.html

x |= (1 << 3);
来源：http://hz.zhijiandao.cn/gtcedybixc.html

[S17] C：安全拼接字符串
来源：http://hz.daxiang520.top/gtmyekibmd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.redwolf501.top/gtskqiplri.html

[S18] C：命令行参数
来源：http://hz.zhoulong.xyz/gtfdzvrjit.html

int main(int argc, char **argv)
来源：http://hz.yvedp.cn/gtkpsxhehw.html

[S19] C：快速排序
来源：http://hz.xziqi.cn/gtdsllszwp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.redwolf501.top/gtxvougwfg.html

[S20] C：二分查找
来源：http://hz.shuidangran.top/gtnqamzzie.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.cqqwz.cn/gtmwleyvas.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gtnzjlxgpk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.316326.xyz/gtvwrioddo.html

[S22] C：字符串转数字
来源：http://hz.tanke756.top/gtsjyrnuml.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.sufxvd.cn/gttajphfjq.html

[S23] C：随机数
来源：http://hz.guannengcc.top/gtaprsogki.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cashguo.top/gthchcgaow.html

[S24] C：获取本地时间
来源：http://hz.xuetiantiany.cn/gtfmemoguk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.jlsjyb.cn/gtownpgyye.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtkyemecil.html

memcpy(dst, src, n);
来源：http://hz.ywan-chungtsiang.top/gthuaaguvz.html

[S26] C：内存清零
来源：http://hz.birdmap.top/gtatpiwodi.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gtgvmuufte.html

[S27] C：定义常量
来源：http://hz.ywan-chungtsiang.top/gtxkqofsbx.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtzphqsynt.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gtkudpxnrp.html

static int counter = 0;
来源：http://hz.chenlongwang.top/gtfegkxved.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtnbeyvacu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.sufxvd.cn/gtpoznewpv.html

[S30] C：头文件保护
来源：http://hz.shangyingyoupin.top/gtecuhqguu.html

#ifndef X_H
来源：http://hz.shzxlz.cn/gttwfpkpzf.html

#define X_H
来源：http://hz.gogol.net.cn/gtjvpcehde.html

#endif
来源：http://hz.gzhubu.top/gttznmqued.html

[S31] C++：Hello World
来源：http://hz.hongshengwenyu.top/gtblfzfsok.html

#include <iostream>
来源：http://hz.52xcode.cn/gtohjdiaan.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.snrcjt.cn/gtqcpbvcpv.html

[S32] C++：字符串
来源：http://hz.jlsjyb.cn/gtalkycxnw.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigfzy.top/gtcpchadth.html

[S33] C++：vector 增删
来源：http://hz.chenzaomai.com/gttoqjaapc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yonumen.top/gtdunkmilm.html

[S34] C++：遍历 vector
来源：http://hz.gotoacloud.top/gtkhszanhj.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenlongwang.top/gtjmpktwhv.html

[S35] C++：map
来源：http://hz.hfpthk.cn/gtogekhplx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinqigfzy.top/gtycemdzpk.html

[S36] C++：unordered_map
来源：http://hz.wangdashe.top/gtuseqycnn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtrvrgcotv.html

[S37] C++：set
来源：http://hz.shanyushiyangtech.top/gttjmtalve.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xuetiantiany.cn/gtzjnzaium.html

[S38] C++：排序
来源：http://hz.zhongyouzk.top/gtgshlysnx.html

std::sort(v.begin(), v.end());
来源：http://hz.nanxinkj.top/gtkkjxlzkr.html

[S39] C++：自定义比较器排序
来源：http://hz.ywan-chungtsiang.top/gtmeynxyts.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.hnqzz.top/gtwhiojpgq.html

[S40] C++：查找元素
来源：http://hz.ydzc1.top/gtmrwcmcjh.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinqigufen.top/gtddgoeorz.html

[S41] C++：类与构造函数
来源：http://hz.daxiang520.top/gtqopcaofb.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.hammf.cn/gthknjpgyu.html

[S42] C++：继承与虚函数
来源：http://hz.nwbrower.top/gtulpkdpfh.html

class B : public Base { public: void f() override {} };
来源：http://hz.xuetiantiany.cn/gtyiporryn.html

[S43] C++：智能指针
来源：http://hz.jinqigufen.top/gtjejfahyd.html

auto p = std::make_unique<int>(5);
来源：http://hz.xziqi.cn/gttwhuxcjn.html

[S44] C++：引用传参
来源：http://hz.bjfxy.top/gtebqsesvd.html

void inc(int &x) { ++x; }
来源：http://hz.birdmap.top/gtatqexecq.html

[S45] C++：lambda
来源：http://hz.chenlongwang.top/gtkbaizvlk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.pycfn.com/gtjdtjozbs.html

[S46] C++：函数模板
来源：http://hz.fzhhl.top/gtrocujqzi.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yj20258.top/gtttjagvls.html

[S47] C++：结构化绑定遍历
来源：http://hz.yonumen.top/gtbawzpvnj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.cashguo.top/gteqmergge.html

[S48] C++：逐行读文件
来源：http://hz.hfpthk.cn/gtbzoizkog.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.ywan-chungtsiang.top/gtokwshsaz.html

while (std::getline(in, line)) { }
来源：http://hz.xuanzx.com/gtvathtpfy.html

[S49] C++：写文件
来源：http://hz.iojbl.cn/gtbalbdylr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.dashuyun.cn/gtsqqrtttk.html

[S50] C++：格式化数字
来源：http://hz.0kj1m.cn/gtfxcowvcv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.svipenyu.cn/gtkesjmbhp.html

[S51] C++：显式类型转换
来源：http://hz.c1oappe.top/gtvjpeejww.html

static_cast<double>(a) / b
来源：http://hz.cashguo.top/gtulhlczpy.html

[S52] C++：const 与 noexcept
来源：http://hz.hnqzz.top/gtycoabpzm.html

int size() const noexcept { return n_; }
来源：http://hz.snrcjt.cn/gtujefpydc.html

[S53] C++：移动语义
来源：http://hz.zhixingplan.top/gtrnjajqqk.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gtxlwnzbia.html

[S54] C++：异常处理
来源：http://hz.yanxiufei.cn/gtksmgqqvt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj202588.top/gtqrowygcp.html

[S55] C++：结构化绑定
来源：http://hz.tian-w.cn/gtzdvkqcoo.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.52xcode.cn/gtwayubuhz.html

[S56] C++：optional
来源：http://hz.cdnleiting.top/gtavfgpzxn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgufenzy.top/gtjhnayteg.html

[S57] C++：编译期常量
来源：http://hz.cheryme.top/gtmktgggcf.html

constexpr int N = 10;
来源：http://hz.0kj1m.cn/gtbvoomfyt.html

[S58] C++：命名空间
来源：http://hz.zdqjudy.top/gtfxibrpev.html

namespace ns { int f() { return 1; } }
来源：http://hz.316326.xyz/gtjkfoxgzx.html

[S59] C++：静态断言
来源：http://hz.yj20258.top/gtizdycvlt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuanzx.com/gtdusdzsvq.html

[S60] C++：遍历并删除元素
来源：http://hz.hnqzz.top/gtadatwsif.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhijiandao.cn/gtcmcvbkjn.html

================================================================================
来源：http://hz.xylfe.cn/gtyldqygme.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.fengsongda.top/gtkeikskth.html

================================================================================
来源：http://hz.snrcjt.cn/gtxcbmhmkk.html

[T01] Kotlin：Hello World
来源：http://hz.fzhhl.top/gtwvztwjyc.html

println("Hello")
来源：http://hz.tanke756.top/gtfgzhpnhf.html

[T02] Kotlin：变量
来源：http://hz.tian-w.cn/gtvcekkvrx.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.cheryme.top/gtejbjkvre.html

[T03] Kotlin：字符串模板
来源：http://hz.xinyue.icu/gtqtyaqrfg.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtbyxknkzu.html

[T04] Kotlin：空安全
来源：http://hz.yj20258.top/gtcrkwhghq.html

val n: String? = null;  n?.length
来源：http://hz.ydjk.org.cn/gtuublrgfj.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtgnjytivn.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.52xcode.cn/gtsbsbbail.html

[T06] Kotlin：集合映射
来源：http://hz.quarkkingdee.top/gtocwtqrqp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hfpthk.cn/gtcogebdoy.html

[T07] Kotlin：集合过滤
来源：http://hz.zhixingplan.top/gtemfzfjhl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.svipenyu.cn/gtddcfrqmu.html

[T08] Kotlin：数据类
来源：http://hz.cdnleiting.top/gtxbbeysso.html

data class User(val name: String, val age: Int)
来源：http://hz.sxryk.cn/gtcdrhbtas.html

[T09] Kotlin：扩展函数
来源：http://hz.kuanghao11.cn/gtrufdmndd.html

fun String.exclaim() = this + "!"
来源：http://hz.yuanzhike.top/gttqflorro.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gtcvydqdyd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258.top/gtonerqpyl.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gtpqnkjjvi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yvedp.cn/gtoomzykwb.html

[T12] Kotlin：解构声明
来源：http://hz.shuidangran.top/gtcrzupgkc.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuxming.cn/gtzvsealrs.html

[T13] Kotlin：只读 Map
来源：http://hz.zhijiandao.cn/gtvonhlvfq.html

val m = mapOf("a" to 1)
来源：http://hz.jinqigufen.top/gtkxaakzzp.html

[T14] Kotlin：循环
来源：http://hz.guannengcc.top/gtmpxjtxmi.html

for (i in 1..10) println(i)
来源：http://hz.chenzaomai.com/gtijgjfkbr.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtktskvyuv.html

interface Shape { fun area(): Double }
来源：http://hz.ywan-chungtsiang.top/gtlmwtuqbq.html

[T16] Swift：Hello World
来源：http://hz.shuidangran.top/gtrosqakdx.html

print("Hello")
来源：http://hz.shuidangran.top/gtxegdufcn.html

[T17] Swift：变量与常量
来源：http://hz.daxiang520.top/gtuxbvqwgv.html

var a = 1;  let b = 2
来源：http://hz.iojbl.cn/gtlxvhrrza.html

[T18] Swift：字符串插值
来源：http://hz.xinyue.icu/gteqbyheor.html

"值: \(b)"
来源：http://hz.zdqjudy.top/gtoasqvtqo.html

[T19] Swift：可选绑定
来源：http://hz.xylfe.cn/gtihuvrsol.html

if let n = opt { print(n) }
来源：http://hz.cucudq.cn/gtleshjuwf.html

[T20] Swift：数组操作
来源：http://hz.haohaochexian.top/gtvjvtgtda.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hywenlv.cn/gtwngmvwqn.html

[T21] Swift：遍历
来源：http://hz.52xcode.cn/gtzgdbtckz.html

for x in a { print(x) }
来源：http://hz.xuanzx.com/gtxxeehvfh.html

[T22] Swift：字典
来源：http://hz.yj20258.top/gtybxuummz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinyuanbaomall.cn/gthkcbtfsc.html

[T23] Swift：函数
来源：http://hz.zhengqikj.top/gtslpdueyu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.jinyuanbaomall.cn/gtrsqnrwqq.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtxgydrlgv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xinyue.icu/gtambyerng.html

[T25] Swift：结构体
来源：http://hz.andypj.xyz/gtnsswjvlf.html

struct P { var x: Int }
来源：http://hz.hnxiangtu.top/gtmjpumvgh.html

[T26] Swift：类与重写
来源：http://hz.ybcxt.top/gtwuiztkbh.html

class A: Base { override func f() {} }
来源：http://hz.vqdsnc.cn/gtoczrgudk.html

[T27] Swift：错误处理
来源：http://hz.ybcxt.top/gtmbzitdmw.html

do { try f() } catch { print(error) }
来源：http://hz.zhiwuduotai.top/gthfgnmtpl.html

[T28] Swift：枚举
来源：http://hz.shzxlz.cn/gtfgkquisw.html

enum Color { case red, green }
来源：http://hz.bjfxy.top/gtkfaltnbr.html

[T29] Swift：guard 提前返回
来源：http://hz.hnqzz.top/gtjpjwblzf.html

guard let x = opt else { return }
来源：http://hz.iojbl.cn/gtdbyunjtu.html

[T30] Swift：协议
来源：http://hz.fzhhl.top/gtyzlibnay.html

protocol Shape { func area() -> Double }
来源：http://hz.fengsongda.top/gtduyzpzny.html


<!-- 参考信息 -->