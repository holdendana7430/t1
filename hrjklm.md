代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.wangshuangyany.cn/gtelftkcue.html

[R26] 命令替换
来源：http://hz.hammf.cn/gtrotaadxl.html

now=$(date +%F); echo "$now"
来源：http://hz.feifeiyinyue.top/gtrqigeeic.html

[R27] 算术展开
来源：http://hz.guowangkeji.top/gtsldnjvmq.html

echo $((1 + 2 * 3))
来源：http://hz.guannengcc.top/gttuenfgco.html

[R28] 浮点运算
来源：http://hz.jlsjyb.cn/gtqritrnnd.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtdrudznfi.html

[R29] 定义函数
来源：http://hz.fzhhl.top/gtornkbwdn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhengqikj.top/gtqahrnjyb.html

[R30] 函数返回状态码
来源：http://hz.zdqjudy.top/gtzxbqfosh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtwsukfube.html

[R31] 局部变量
来源：http://hz.xuetiantiany.cn/gtlsejkuge.html

f() { local x=1; echo "$x"; }
来源：http://hz.hammf.cn/gtnpeswiag.html

[R32] 参数个数校验
来源：http://hz.cdnleiting.top/gtdpqchrzc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.guannengcc.top/gtduggojmu.html

[R33] 捕获错误并提示行号
来源：http://hz.yueranfly.top/gtfypztvka.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gtldnkwydk.html

[R34] 退出时清理
来源：http://hz.xylfe.cn/gtrmitueny.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtyourkdle.html

[R35] 后台执行并等待
来源：http://hz.snrcjt.cn/gtxslivqxh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hnqzz.top/gtdhewyecp.html

[R36] 并发执行多个任务
来源：http://hz.jqgufenzy.top/gticexwcau.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258.top/gtpkbqvkdv.html

[R37] 把输出赋给变量
来源：http://hz.xylfe.cn/gtbcwzuvvh.html

files=$(ls -1)
来源：http://hz.ehwqpu.com/gtvwmkqeaw.html

[R38] 管道串联
来源：http://hz.52xcode.cn/gtvltzhwzb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ppjwa.cn/gtksoysyou.html

[R39] 重定向标准输出与错误
来源：http://hz.shanyushiyangkeji.top/gtrcukkeve.html

cmd > out.log 2>&1
来源：http://hz.yueranfly.top/gtgckmakrb.html

[R40] 追加写日志
来源：http://hz.hfpthk.cn/gtlkarqeuf.html

echo "log" >> out.log
来源：http://hz.cucudq.cn/gtkucvopij.html

[R41] 丢弃输出
来源：http://hz.jiagoushi.top/gtfblptqkt.html

cmd >/dev/null 2>&1
来源：http://hz.jianghu66.top/gtkpqpiyqw.html

[R42] 输入重定向
来源：http://hz.cqqwz.cn/gtlguaovdx.html

wc -l < a.txt
来源：http://hz.aibaodan.cn/gtntafngap.html

[R43] 按名字查找文件
来源：http://hz.tian-w.cn/gtzvqqmeok.html

find . -name "*.log" -type f
来源：http://hz.ivvv.top/gtrkocjvpf.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtmtsubysj.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtoabbcfoc.html

[R45] 批量删除
来源：http://hz.zhixingplan.top/gtempcbnbb.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtrwicazbn.html

[R46] 递归替换文件内容
来源：http://hz.birdmap.top/gtxxjwzhzs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cucudq.cn/gtubrcgnlq.html

[R47] sed 单行替换
来源：http://hz.gaohongyu789.top/gtwblojarl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tian-w.cn/gtehqmymjp.html

[R48] awk 取指定列
来源：http://hz.shzxlz.cn/gtmcequqye.html

awk '{print $1, $3}' a.txt
来源：http://hz.cqqwz.cn/gtbhpzwznd.html

[R49] awk 带条件
来源：http://hz.chenlongwang.top/gtzbzhvaqr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ivvv.top/gtnokaxjgt.html

[R50] awk 求和
来源：http://hz.cashguo.top/gtbfgambsu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtunilynnj.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtvsjrrrcw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.tianlin.xyz/gtupgnavxm.html

[R52] 统计行数
来源：http://hz.xziqi.cn/gtquuctwwx.html

wc -l a.txt
来源：http://hz.birdmap.top/gtevldckxg.html

[R53] 查看文件头与实时尾
来源：http://hz.jinqigufen.top/gttnzqewgd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtttcobkmc.html

[R54] 比较两个文件
来源：http://hz.zdqjudy.top/gtvuqpbayu.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gteywjpopc.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtgaudcrqz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.aibaodan.cn/gtqvsxookb.html

[R56] 远程拷贝
来源：http://hz.fengsongda.top/gtbaaljlpm.html

scp file user@host:/path/
来源：http://hz.yj20258888.top/gtwsnxjomk.html

[R57] 远程执行命令
来源：http://hz.chenlongwang.top/gtswgerzfd.html

ssh user@host 'uptime'
来源：http://hz.ppjwa.cn/gtfouvtcfd.html

[R58] 下载文件
来源：http://hz.aizwys.cn/gtwicfgrzq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shzxlz.cn/gtayvpawnu.html

[R59] 发 POST JSON
来源：http://hz.jlsjyb.cn/gtegpteahj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yangfankeji.com/gtyajwedjf.html

[R60] 只看 HTTP 状态码
来源：http://hz.fzhhl.top/gthdtitbgu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sufxvd.cn/gtdkgwwibb.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtxeetpzyj.html

df -h;  du -sh *
来源：http://hz.wangdashe.top/gtvndvfcfu.html

[R62] 找最占空间的文件
来源：http://hz.ppjwa.cn/gtwseomhwu.html

du -ah . | sort -rh | head -10
来源：http://hz.iojbl.cn/gtifugcznz.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtelzikoye.html

free -h;  ps aux | grep nginx
来源：http://hz.ehwqpu.com/gtfsxksfrm.html

[R64] 结束进程
来源：http://hz.ywan-chungtsiang.top/gtntwmnjwh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtxuznckym.html

[R65] 查看端口占用
来源：http://hz.hnxiangtu.top/gticmbdkix.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtbmtwqevl.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtlranxalr.html

crontab -e;  crontab -l
来源：http://hz.xuanzx.com/gtrpceycwu.html

[R67] 生成随机十六进制串
来源：http://hz.guowangkeji.top/gtgsvabfrc.html

openssl rand -hex 16
来源：http://hz.cashguo.top/gtkdxowqtx.html

[R68] 计算文件校验值
来源：http://hz.xuetiantiany.cn/gttlsxqrjc.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.shanyushiyangtech.top/gtmdtrztgg.html

[R69] 生成随机密码
来源：http://hz.0kj1m.cn/gtgmrfjako.html

head -c 16 /dev/urandom | base64
来源：http://hz.sweek.top/gtisfcrqns.html

[R70] 时间戳与互转
来源：http://hz.zdqjudy.top/gtazbdrpbg.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gtjnadswdd.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gtijtwjlbk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guannengcc.top/gtmafiixif.html

[R72] 等待端口就绪
来源：http://hz.hnqzz.top/gtgovouolp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jyoumei.cn/gtkbykatsb.html

[R73] 分割大日志
来源：http://hz.shanyushiyangtech.top/gthyaakkwv.html

split -l 1000 big.log part_
来源：http://hz.birdmap.top/gtqgqvzdmu.html

[R74] 批量重命名
来源：http://hz.iojbl.cn/gtvvsvxdub.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yueranfly.top/gtcszfpvrt.html

[R75] 导出环境变量
来源：http://hz.wangdashe.top/gtmhnohbcf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.redwolf501.top/gtgpxcntjj.html

[R76] 使用临时文件
来源：http://hz.bjfxy.top/gtrncvsttv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.zdqjudy.top/gtbiqdtvoh.html

[R77] 读取用户输入
来源：http://hz.yongpay.top/gtywixflkw.html

read -rp "请输入: " ans
来源：http://hz.tian-w.cn/gtzcuwavxo.html

[R78] 交互式菜单
来源：http://hz.jyoumei.cn/gtiswzqgcu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgufenzy.top/gttetuzlqz.html

[R79] 解析命令行选项
来源：http://hz.cashguo.top/gtsittxvoe.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtlsdeeyko.html

[R80] 查看脚本执行耗时
来源：http://hz.haohaochexian.top/gtswnhrwjz.html

time ./run.sh
来源：http://hz.ehwqpu.com/gtizkopsly.html

================================================================================
来源：http://hz.shangyingyoupin.top/gttcpzkmhh.html

S. C / C++ 专题
来源：http://hz.hnqzz.top/gtjoubtljz.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtvciysgvp.html

[S01] C：Hello World
来源：http://hz.chenlongwang.top/gtavnnxboo.html

#include <stdio.h>
来源：http://hz.shanyushiyangkeji.top/gthqsfrbmb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gtyzwcyigw.html

[S02] C：变量与格式化输出
来源：http://hz.jinyuanbaomall.cn/gthbkzayro.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gthykyldjv.html

[S03] C：读入整数
来源：http://hz.gaohongyu789.top/gtinlpnloa.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtnnfmsrjf.html

[S04] C：字符串复制
来源：http://hz.chenjidiqi.icu/gtppmebpec.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.snrcjt.cn/gtsjbntdnv.html

[S05] C：字符串长度
来源：http://hz.hysaishi.cn/gtmqiuyohq.html

strlen(s)
来源：http://hz.tianlin.xyz/gtqqxytyss.html

[S06] C：字符串比较
来源：http://hz.jinqigfzy.top/gtuemhrjik.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gtsztjsudm.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtfagbngbw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gogol.net.cn/gtaujlhgll.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtqanjtntv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtydhbqywt.html

[S09] C：结构体定义与初始化
来源：http://hz.kuanghao11.cn/gttfneymts.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tianlin.xyz/gtyfkwepux.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gtvgdgqejk.html

int *p = &a;  *p = 5;
来源：http://hz.jyoumei.cn/gthstnfxlb.html

[S11] C：逐行读文件
来源：http://hz.shanyushiyangtech.top/gtdrhwmctf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gtizwgdejt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.316326.xyz/gtifyfityy.html

fclose(f);
来源：http://hz.yj202588.top/gtjqsuxfke.html

[S12] C：写文件
来源：http://hz.guowangkeji.top/gtvmirugry.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.snrcjt.cn/gtnbsgyslk.html

[S13] C：宏定义
来源：http://hz.bjfxy.top/gtxdwqrsbp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtuwqumfoz.html

[S14] C：枚举
来源：http://hz.shanyushiyangtech.top/gtekjeiwdj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.pengpengdd.cyou/gtjnwsncea.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtoovngxdg.html

(double) a / b
来源：http://hz.jinqigfzy.top/gtaasukjrc.html

[S16] C：位操作置位
来源：http://hz.ppjwa.cn/gtgoduyeml.html

x |= (1 << 3);
来源：http://hz.havefunace.top/gtjcqkutjd.html

[S17] C：安全拼接字符串
来源：http://hz.gzhubu.top/gtbjkneryh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ehwqpu.com/gtqdaihchs.html

[S18] C：命令行参数
来源：http://hz.dashuyun.cn/gtnjzkyxtu.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtebchyfyb.html

[S19] C：快速排序
来源：http://hz.zhoulong.xyz/gtzmbwwxai.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtratasqcv.html

[S20] C：二分查找
来源：http://hz.guowangkeji.top/gtffyhlyvp.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.smart0.xyz/gtdmmxdxhf.html

[S21] C：字符类别判断
来源：http://hz.tianlin.xyz/gtujbneqas.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ybcxt.top/gtmcduxgxt.html

[S22] C：字符串转数字
来源：http://hz.nanxuanxn.top/gtphpwuzfd.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yueranfly.top/gtvfnsroli.html

[S23] C：随机数
来源：http://hz.xuanzx.com/gtgflozrig.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.zhixingplan.top/gtkgaqpfxz.html

[S24] C：获取本地时间
来源：http://hz.haohaochexian.top/gtcpgzwwyt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhixingplan.top/gtyojfqkxq.html

[S25] C：内存拷贝
来源：http://hz.chenlongwang.top/gtyigektrh.html

memcpy(dst, src, n);
来源：http://hz.wangshuangyany.cn/gtwgbzcazq.html

[S26] C：内存清零
来源：http://hz.nanxuanxn.top/gtbbmohauj.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258.top/gthxfflxie.html

[S27] C：定义常量
来源：http://hz.chenlongwang.top/gtghosyfgb.html

const double PI = 3.14159;
来源：http://hz.sysykeji.top/gtfjiwmfkx.html

[S28] C：静态变量
来源：http://hz.tianlin.xyz/gttfnozamu.html

static int counter = 0;
来源：http://hz.zhoulong.xyz/gttoxmwexg.html

[S29] C：变参函数
来源：http://hz.sysykeji.top/gtvfejrfyq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cashguo.top/gtywhlluip.html

[S30] C：头文件保护
来源：http://hz.sysykeji.top/gtlewwxsnh.html

#ifndef X_H
来源：http://hz.fzhhl.top/gtxjcfjwnb.html

#define X_H
来源：http://hz.haohaochexian.top/gtdetxnuzp.html

#endif
来源：http://hz.gaohongyu789.top/gtpjmwirsf.html

[S31] C++：Hello World
来源：http://hz.zhixingplan.top/gtexlilxzc.html

#include <iostream>
来源：http://hz.jqgufenzy.top/gtiryukzke.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.iojbl.cn/gtkdsrcluv.html

[S32] C++：字符串
来源：http://hz.cqqwz.cn/gtwjnoktrl.html

std::string s = "hi";  s += "!";
来源：http://hz.guannengcc.top/gttkwvojzc.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gtnpnztixx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.xinyue.icu/gtwaxjpwrk.html

[S34] C++：遍历 vector
来源：http://hz.sysykeji.top/gtcuaqflol.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtovxgxhgj.html

[S35] C++：map
来源：http://hz.pycfn.com/gtclbanvug.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yongpay.top/gtpuezpbsd.html

[S36] C++：unordered_map
来源：http://hz.tanke756.top/gtrzpvlaxp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hfpthk.cn/gtrljkgnwj.html

[S37] C++：set
来源：http://hz.tian-w.cn/gtcshheode.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtvyksljos.html

[S38] C++：排序
来源：http://hz.yonumen.top/gtjktuflpe.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gtnqqbndlf.html

[S39] C++：自定义比较器排序
来源：http://hz.snrcjt.cn/gtgahaidmh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zdqjudy.top/gtqwrikfqg.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gtejumgzjb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.guowangkeji.top/gtqgegtnep.html

[S41] C++：类与构造函数
来源：http://hz.shzxlz.cn/gtzwumygmw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.andypj.xyz/gtqniqblzf.html

[S42] C++：继承与虚函数
来源：http://hz.smart0.xyz/gthjvlszac.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenjidiqi.icu/gtafnclxwc.html

[S43] C++：智能指针
来源：http://hz.yueranfly.top/gtcwvmcofr.html

auto p = std::make_unique<int>(5);
来源：http://hz.ppjwa.cn/gtrhaboley.html

[S44] C++：引用传参
来源：http://hz.zdqjudy.top/gtyoiajjxz.html

void inc(int &x) { ++x; }
来源：http://hz.ehwqpu.com/gtemdrqjek.html

[S45] C++：lambda
来源：http://hz.tian-w.cn/gtspqcrbjk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtnvnqvopl.html

[S46] C++：函数模板
来源：http://hz.nwbrower.top/gtuuefalwq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtzpxflvvx.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258888.top/gttconpilq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jiagoushi.top/gtppbirnth.html

[S48] C++：逐行读文件
来源：http://hz.mhx1999.top/gtcbbhcimq.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hnxiangtu.top/gtuelfiagw.html

while (std::getline(in, line)) { }
来源：http://hz.jiagoushi.top/gtiyfqgoog.html

[S49] C++：写文件
来源：http://hz.shangyingyoupin.top/gtvfbjzwcm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.gaohongyu789.top/gtkwbacwsl.html

[S50] C++：格式化数字
来源：http://hz.jinqigufen.top/gtijaljqwm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jianghu66.top/gtpjrsslbi.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtiyeqtyim.html

static_cast<double>(a) / b
来源：http://hz.jianghu66.top/gtfxzmjksg.html

[S52] C++：const 与 noexcept
来源：http://hz.shanyushiyangtech.top/gtvfftrxsz.html

int size() const noexcept { return n_; }
来源：http://hz.xziqi.cn/gtzekvhpgm.html

[S53] C++：移动语义
来源：http://hz.havefunace.top/gtnqjlshqu.html

std::vector<int> w = std::move(v);
来源：http://hz.cqqwz.cn/gtzirfjvxd.html

[S54] C++：异常处理
来源：http://hz.zhijiandao.cn/gthylzyirn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hfpthk.cn/gthwvdyjbf.html

[S55] C++：结构化绑定
来源：http://hz.yj20258888.top/gtoqledtkl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigufen.top/gtvwvoybjp.html

[S56] C++：optional
来源：http://hz.dashuyun.cn/gtnajxzfug.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.316326.xyz/gtacqdqdec.html

[S57] C++：编译期常量
来源：http://hz.0kj1m.cn/gtwqozzjte.html

constexpr int N = 10;
来源：http://hz.havefunace.top/gtgedyuihb.html

[S58] C++：命名空间
来源：http://hz.sweek.top/gtpyopfosc.html

namespace ns { int f() { return 1; } }
来源：http://hz.ydjk.org.cn/gtuwalsufo.html

[S59] C++：静态断言
来源：http://hz.ywan-chungtsiang.top/gttdzpfnsb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.ivvv.top/gtnepjksax.html

[S60] C++：遍历并删除元素
来源：http://hz.jyoumei.cn/gtvaduivpr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.zhixingplan.top/gtgvwrrrhx.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtmjnmwbfy.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtvyjehlhl.html

================================================================================
来源：http://hz.tianlin.xyz/gtkowohxcj.html

[T01] Kotlin：Hello World
来源：http://hz.jyoumei.cn/gtfhhmhhtw.html

println("Hello")
来源：http://hz.fzhhl.top/gtqrwxrnir.html

[T02] Kotlin：变量
来源：http://hz.yj202588.top/gtmgfexbxa.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.birdmap.top/gtlofhfvnz.html

[T03] Kotlin：字符串模板
来源：http://hz.hywenlv.cn/gtmarjzsnv.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtyszsxukd.html

[T04] Kotlin：空安全
来源：http://hz.zhiwuduotai.top/gtnuobmqsi.html

val n: String? = null;  n?.length
来源：http://hz.yanxiufei.cn/gtzcbhhuer.html

[T05] Kotlin：when 表达式
来源：http://hz.yj20258888.top/gtzkohdpaa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jianghu66.top/gtsbswjshm.html

[T06] Kotlin：集合映射
来源：http://hz.yueranfly.top/gtftzabzfz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jinghuilouyu.cn/gtlnoevzft.html

[T07] Kotlin：集合过滤
来源：http://hz.ivvv.top/gtbmgogila.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.zhixingplan.top/gtqeecnwqz.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtvnhsloho.html

data class User(val name: String, val age: Int)
来源：http://hz.gaohongyu789.top/gttpcqjwns.html

[T09] Kotlin：扩展函数
来源：http://hz.nwbrower.top/gtbqlmqgss.html

fun String.exclaim() = this + "!"
来源：http://hz.yonumen.top/gtfeqfjmia.html

[T10] Kotlin：默认参数
来源：http://hz.guannengcc.top/gtorrvjxbb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yongpay.top/gtuzwgixdg.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtvrofgeij.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dianchejie.cn/gtkdnelzxy.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtbuklrazm.html

val (a, b) = Pair(1, 2)
来源：http://hz.haohaochexian.top/gtkjqsujyb.html

[T13] Kotlin：只读 Map
来源：http://hz.xinyue.icu/gtmklzzduy.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gteuaiwvqx.html

[T14] Kotlin：循环
来源：http://hz.xziqi.cn/gtxradubrm.html

for (i in 1..10) println(i)
来源：http://hz.316326.xyz/gthutxoook.html

[T15] Kotlin：接口
来源：http://hz.ydjk.org.cn/gttipfrjuu.html

interface Shape { fun area(): Double }
来源：http://hz.zhoulong.xyz/gtjdjwdfrr.html

[T16] Swift：Hello World
来源：http://hz.cdnleiting.top/gtnustbsor.html

print("Hello")
来源：http://hz.zhengqikj.top/gtimyhdpyj.html

[T17] Swift：变量与常量
来源：http://hz.xuanzx.com/gtwunxoftd.html

var a = 1;  let b = 2
来源：http://hz.shanyushiyangkeji.top/gtkesrzibp.html

[T18] Swift：字符串插值
来源：http://hz.meibo888.top/gttjqrwjal.html

"值: \(b)"
来源：http://hz.cqqwz.cn/gtoiepojss.html

[T19] Swift：可选绑定
来源：http://hz.snrcjt.cn/gtepgmfbdi.html

if let n = opt { print(n) }
来源：http://hz.52xcode.cn/gtkmgbrbpw.html

[T20] Swift：数组操作
来源：http://hz.jinqigfzy.top/gtucrupuch.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tianlin.xyz/gtgjnegabv.html

[T21] Swift：遍历
来源：http://hz.gogol.net.cn/gthgiukxdi.html

for x in a { print(x) }
来源：http://hz.aibaodan.cn/gtwkgdjphv.html

[T22] Swift：字典
来源：http://hz.hysaishi.cn/gtenpouwxv.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.9152youxi.cn/gthaxphiqm.html

[T23] Swift：函数
来源：http://hz.jiagoushi.top/gteckdozeh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.xinyue.icu/gtqrmafocv.html

[T24] Swift：闭包
来源：http://hz.xylfe.cn/gtbipvcihp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gogol.net.cn/gtdqtnmgcy.html

[T25] Swift：结构体
来源：http://hz.fengsongda.top/gtdklpkzlz.html

struct P { var x: Int }
来源：http://hz.gotoacloud.top/gtgqplwkhz.html

[T26] Swift：类与重写
来源：http://hz.zhixingplan.top/gtvynxotph.html

class A: Base { override func f() {} }
来源：http://hz.ydzc1.top/gtgkdhtpmx.html

[T27] Swift：错误处理
来源：http://hz.kuanghao11.cn/gtpcmtkinq.html

do { try f() } catch { print(error) }
来源：http://hz.sufxvd.cn/gtjfypcyqt.html

[T28] Swift：枚举
来源：http://hz.jinqigfzy.top/gtgwubojgd.html

enum Color { case red, green }
来源：http://hz.gogol.net.cn/gtpvbiimrk.html


<!-- 参考信息 -->