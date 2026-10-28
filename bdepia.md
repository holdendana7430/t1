代发 wailian999

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.c1oappe.top/gthcywilir.html

[R30] 函数返回状态码
来源：http://hz.pengpengdd.cyou/gtoprmxhcu.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hongshengwenyu.top/gtdlaplgho.html

[R31] 局部变量
来源：http://hz.aizwys.cn/gtxgzrlpal.html

f() { local x=1; echo "$x"; }
来源：http://hz.yonumen.top/gtxfbnqbuz.html

[R32] 参数个数校验
来源：http://hz.feifeiyinyue.top/gtjugdmmlo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtdosfuhux.html

[R33] 捕获错误并提示行号
来源：http://hz.yuanzhike.top/gtgroizwia.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.feifeiyinyue.top/gttebuqjot.html

[R34] 退出时清理
来源：http://hz.smart0.xyz/gtwfjaxkxl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtflivmmwp.html

[R35] 后台执行并等待
来源：http://hz.jyoumei.cn/gtsncmgijc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gtoozliznn.html

[R36] 并发执行多个任务
来源：http://hz.xinyue.icu/gtdklhvlnm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yangfankeji.com/gtyixppghw.html

[R37] 把输出赋给变量
来源：http://hz.pycfn.com/gtiyuyjfsi.html

files=$(ls -1)
来源：http://hz.zhixingplan.top/gtyrbaipsi.html

[R38] 管道串联
来源：http://hz.zhiwuduotai.top/gtezjgxgtr.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xuanzx.com/gtvqnnryqh.html

[R39] 重定向标准输出与错误
来源：http://hz.ybcxt.top/gtwqxwsrwe.html

cmd > out.log 2>&1
来源：http://hz.0kj1m.cn/gthgtojwxg.html

[R40] 追加写日志
来源：http://hz.shangyingyoupin.top/gtgqovilar.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtqhdeexpo.html

[R41] 丢弃输出
来源：http://hz.hnxiangtu.top/gtqxwngyka.html

cmd >/dev/null 2>&1
来源：http://hz.zhijiandao.cn/gtqwitcwgu.html

[R42] 输入重定向
来源：http://hz.zhijiandao.cn/gtqbodjrdb.html

wc -l < a.txt
来源：http://hz.zhiwuduotai.top/gtrmehtjoq.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangtech.top/gtewvqlmto.html

find . -name "*.log" -type f
来源：http://hz.svipenyu.cn/gtqfxxgkex.html

[R44] 按修改时间查找
来源：http://hz.sufxvd.cn/gtyhcgxahs.html

find . -mtime -7 -type f
来源：http://hz.sufxvd.cn/gtlmljrrvr.html

[R45] 批量删除
来源：http://hz.meibo888.top/gtjjupqrne.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtondndtdb.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gteneytnnj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jqgfzy.top/gtzkrhqqbc.html

[R47] sed 单行替换
来源：http://hz.shuidangran.top/gttvhncqfa.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.shanyushiyangtech.top/gtrezwtxrf.html

[R48] awk 取指定列
来源：http://hz.quarkkingdee.top/gtmnoxttxd.html

awk '{print $1, $3}' a.txt
来源：http://hz.zdqjudy.top/gtupdjbpom.html

[R49] awk 带条件
来源：http://hz.chenzaomai.com/gtfnbnmbhu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.yueranfly.top/gtzhnqmsme.html

[R50] awk 求和
来源：http://hz.cqqwz.cn/gtqhdhjvdw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.svipenyu.cn/gtdzwuujat.html

[R51] 排序去重取前几
来源：http://hz.pengpengdd.cyou/gtzjqwktks.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yonumen.top/gtqchaqkrt.html

[R52] 统计行数
来源：http://hz.ivvv.top/gtbzhyftff.html

wc -l a.txt
来源：http://hz.feifeiyinyue.top/gtnbmymfev.html

[R53] 查看文件头与实时尾
来源：http://hz.shzxlz.cn/gtokbhgitu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yvedp.cn/gtustkaynn.html

[R54] 比较两个文件
来源：http://hz.birdmap.top/gtzrsedack.html

diff a.txt b.txt
来源：http://hz.xziqi.cn/gtjleerghk.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtpkraswnk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hysaishi.cn/gtmrbtqnjl.html

[R56] 远程拷贝
来源：http://hz.sufxvd.cn/gtlrucfski.html

scp file user@host:/path/
来源：http://hz.chenlongwang.top/gtwlnvhuxd.html

[R57] 远程执行命令
来源：http://hz.fengsongda.top/gtsvqobiuw.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtvgeersty.html

[R58] 下载文件
来源：http://hz.ywan-chungtsiang.top/gtlbfuizef.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.gaohongyu789.top/gthjuppkeo.html

[R59] 发 POST JSON
来源：http://hz.zhiwuduotai.top/gtpvuwtomg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhoulong.xyz/gtocphvdxx.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhongyouzk.top/gtvxiikmct.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shangyingyoupin.top/gtryanqclk.html

[R61] 磁盘占用
来源：http://hz.daxiang520.top/gtodvlilrj.html

df -h;  du -sh *
来源：http://hz.cdnleiting.top/gtusrxfdaw.html

[R62] 找最占空间的文件
来源：http://hz.cucudq.cn/gtnrgfkhdg.html

du -ah . | sort -rh | head -10
来源：http://hz.svipenyu.cn/gtjzoaylfs.html

[R63] 内存与进程
来源：http://hz.gogol.net.cn/gthzjhhplh.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangkeji.top/gtfdaybced.html

[R64] 结束进程
来源：http://hz.zdqjudy.top/gthqmjcelx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.kuanghao11.cn/gtihvtafpo.html

[R65] 查看端口占用
来源：http://hz.wangdashe.top/gtkydrteap.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tianlin.xyz/gtsjbyjbfk.html

[R66] 定时任务
来源：http://hz.jyoumei.cn/gtbspqlszw.html

crontab -e;  crontab -l
来源：http://hz.zhoulong.xyz/gtnffevyfn.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtwnpvptpw.html

openssl rand -hex 16
来源：http://hz.shanyushiyangtech.top/gtxsopiotc.html

[R68] 计算文件校验值
来源：http://hz.feifeiyinyue.top/gtogjifafm.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yuanzhike.top/gtjzgvrzke.html

[R69] 生成随机密码
来源：http://hz.yueranfly.top/gtbdszupke.html

head -c 16 /dev/urandom | base64
来源：http://hz.gzhubu.top/gtuidxburl.html

[R70] 时间戳与互转
来源：http://hz.zhiwuduotai.top/gtkoghmsqe.html

date +%s;  date -d @1700000000
来源：http://hz.chenzaomai.com/gtamnlvjcc.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gtrgbrpdoy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.hnxiangtu.top/gtcqsvxwor.html

[R72] 等待端口就绪
来源：http://hz.meibo888.top/gtlsveoopc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yj20258.top/gtqgrzoira.html

[R73] 分割大日志
来源：http://hz.bjfxy.top/gtazakjjkl.html

split -l 1000 big.log part_
来源：http://hz.tianlin.xyz/gtmqgkzuhm.html

[R74] 批量重命名
来源：http://hz.wangdashe.top/gtwuqcwvln.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xziqi.cn/gtlcdsiycf.html

[R75] 导出环境变量
来源：http://hz.ehwqpu.com/gtmlgmxcvb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigufen.top/gtrsrkykxx.html

[R76] 使用临时文件
来源：http://hz.yj20258.top/gtgutgbhyl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.kuanghao11.cn/gtivvjqxqe.html

[R77] 读取用户输入
来源：http://hz.wangshuangyany.cn/gtactjdind.html

read -rp "请输入: " ans
来源：http://hz.dashuyun.cn/gtlcrvmbrh.html

[R78] 交互式菜单
来源：http://hz.ppjwa.cn/gtdexgwbbb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigufen.top/gtkliyhzwe.html

[R79] 解析命令行选项
来源：http://hz.yonumen.top/gtbxnpsfpz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gtfmkftkms.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gttjtoqcqk.html

time ./run.sh
来源：http://hz.redwolf501.top/gtgkhtczvc.html

================================================================================
来源：http://hz.xylfe.cn/gtzeelmili.html

S. C / C++ 专题
来源：http://hz.zhaomingkeji.xyz/gtdyipxcew.html

================================================================================
来源：http://hz.zhoulong.xyz/gtaynexzli.html

[S01] C：Hello World
来源：http://hz.yuxming.cn/gttkucttky.html

#include <stdio.h>
来源：http://hz.chenjidiqi.icu/gtuprwoptn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinyuanbaomall.cn/gtyvfrimxw.html

[S02] C：变量与格式化输出
来源：http://hz.zhengqikj.top/gticowadfg.html

int a = 10; printf("%d\n", a);
来源：http://hz.shanyushiyangkeji.top/gtxncvdrpn.html

[S03] C：读入整数
来源：http://hz.jinqigufen.top/gtqlckstmn.html

int x; scanf("%d", &x);
来源：http://hz.zhaomingkeji.xyz/gtqxbucxdh.html

[S04] C：字符串复制
来源：http://hz.gotoacloud.top/gtiqmgccpz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xinyue.icu/gtluqsxkqi.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtniuqrgug.html

strlen(s)
来源：http://hz.ehwqpu.com/gtlwghocio.html

[S06] C：字符串比较
来源：http://hz.hnqzz.top/gtzzwfyekm.html

strcmp(a, b) == 0
来源：http://hz.quarkkingdee.top/gtmxxizgvc.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtghzimhob.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tianlin.xyz/gtjjnkemqf.html

[S08] C：动态内存分配与释放
来源：http://hz.sysykeji.top/gtypysgrvn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinghuilouyu.cn/gtunmspedm.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gteybrxseb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.shangyingyoupin.top/gtkgswjxuy.html

[S10] C：指针与解引用
来源：http://hz.feifeiyinyue.top/gtzhrxfxhi.html

int *p = &a;  *p = 5;
来源：http://hz.guowangkeji.top/gtfempnehd.html

[S11] C：逐行读文件
来源：http://hz.zycfv.cn/gtcgryxkmc.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtmtvzuqpm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhengqikj.top/gthqrknder.html

fclose(f);
来源：http://hz.aizwys.cn/gtianafzky.html

[S12] C：写文件
来源：http://hz.cqqwz.cn/gtalabhqgq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gaohongyu789.top/gtoxjqkfud.html

[S13] C：宏定义
来源：http://hz.cqqwz.cn/gtxyglsztm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.birdmap.top/gtahixvqkp.html

[S14] C：枚举
来源：http://hz.vqdsnc.cn/gtjqzeivpw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gteowkjcmf.html

[S15] C：类型转换
来源：http://hz.hywenlv.cn/gttcuxbcuz.html

(double) a / b
来源：http://hz.wangshuangyany.cn/gtgvpftmfb.html

[S16] C：位操作置位
来源：http://hz.guowangkeji.top/gtrybmuvte.html

x |= (1 << 3);
来源：http://hz.pengpengdd.cyou/gtczqwasec.html

[S17] C：安全拼接字符串
来源：http://hz.cqqwz.cn/gtpuwuygmk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.feifeiyinyue.top/gtkajqairo.html

[S18] C：命令行参数
来源：http://hz.yueranfly.top/gtpluzixzu.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtfqcynhee.html

[S19] C：快速排序
来源：http://hz.feifeiyinyue.top/gtjcpwfqwt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtouqkwrjl.html

[S20] C：二分查找
来源：http://hz.hongshengwenyu.top/gtweyrezlh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtqawghhoe.html

[S21] C：字符类别判断
来源：http://hz.gotoacloud.top/gttmggbqeo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydzc1.top/gtpdccwalq.html

[S22] C：字符串转数字
来源：http://hz.zhaomingkeji.xyz/gtwqexkfzz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shanyushiyangtech.top/gtjgwqtzbp.html

[S23] C：随机数
来源：http://hz.zycfv.cn/gtgcutiltp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xingfuxueyuan.xyz/gtfgtjhipv.html

[S24] C：获取本地时间
来源：http://hz.9152youxi.cn/gtxgbbzkda.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtywxeuviw.html

[S25] C：内存拷贝
来源：http://hz.yuxming.cn/gtrngpybcu.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtyhrpjmgi.html

[S26] C：内存清零
来源：http://hz.ppjwa.cn/gtkfsreftx.html

memset(a, 0, sizeof a);
来源：http://hz.yj20258.top/gtdsomwpvf.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtbvcikwpj.html

const double PI = 3.14159;
来源：http://hz.yangfankeji.com/gtplvtioaf.html

[S28] C：静态变量
来源：http://hz.redwolf501.top/gtkcwtwesu.html

static int counter = 0;
来源：http://hz.sysykeji.top/gtleyvjcnj.html

[S29] C：变参函数
来源：http://hz.chenjidiqi.icu/gtydakxego.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hammf.cn/gtuexvfati.html

[S30] C：头文件保护
来源：http://hz.dianchejie.cn/gteyirjmzk.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtfeuxtvfk.html

#define X_H
来源：http://hz.hnxiangtu.top/gtlltrrrin.html

#endif
来源：http://hz.aizwys.cn/gtbwopeyyi.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtppbtbgwa.html

#include <iostream>
来源：http://hz.ehwqpu.com/gtonajbwxx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj20258.top/gtgzjggrxh.html

[S32] C++：字符串
来源：http://hz.birdmap.top/gtdbffqlws.html

std::string s = "hi";  s += "!";
来源：http://hz.chenzaomai.com/gtdpdueggi.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gtlwzuzffi.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gtvwnbxcwg.html

[S34] C++：遍历 vector
来源：http://hz.sufxvd.cn/gtqeytxahb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.pengpengdd.cyou/gtgmcaqbix.html

[S35] C++：map
来源：http://hz.52xcode.cn/gtagnppcbe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dashuyun.cn/gtdqipwovx.html

[S36] C++：unordered_map
来源：http://hz.smart0.xyz/gtxeyedffm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtgiwdrxyx.html

[S37] C++：set
来源：http://hz.zhixingplan.top/gtnvogdbpf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.yvedp.cn/gtmgvrnpeh.html

[S38] C++：排序
来源：http://hz.xinyue.icu/gtrhtrdaun.html

std::sort(v.begin(), v.end());
来源：http://hz.snrcjt.cn/gtkxfzmznc.html

[S39] C++：自定义比较器排序
来源：http://hz.xuetiantiany.cn/gtlrcmryrt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.mhx1999.top/gtbbqpwppn.html

[S40] C++：查找元素
来源：http://hz.hfpthk.cn/gtxjkgwubc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jiagoushi.top/gtqmczsjbg.html

[S41] C++：类与构造函数
来源：http://hz.tianlin.xyz/gtwogevvcm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tianlin.xyz/gtualjsaoj.html

[S42] C++：继承与虚函数
来源：http://hz.daxiang520.top/gtoknvwvjj.html

class B : public Base { public: void f() override {} };
来源：http://hz.snrcjt.cn/gtklkcbumr.html

[S43] C++：智能指针
来源：http://hz.guannengcc.top/gtgqojlaud.html

auto p = std::make_unique<int>(5);
来源：http://hz.yueranfly.top/gtpoqyfyfr.html

[S44] C++：引用传参
来源：http://hz.jyoumei.cn/gtxkrdqunb.html

void inc(int &x) { ++x; }
来源：http://hz.nanxinkj.top/gtwrurqpcr.html

[S45] C++：lambda
来源：http://hz.feifeiyinyue.top/gtuaylcnco.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.dianchejie.cn/gtjepihbrz.html

[S46] C++：函数模板
来源：http://hz.mhx1999.top/gtcsltgyfd.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tian-w.cn/gtrfnntgpe.html

[S47] C++：结构化绑定遍历
来源：http://hz.cdnleiting.top/gtpacxconz.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtbepcmmzw.html

[S48] C++：逐行读文件
来源：http://hz.aibaodan.cn/gtzbalraet.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jiagoushi.top/gtspfbnjgc.html

while (std::getline(in, line)) { }
来源：http://hz.cqqwz.cn/gtgatrrmwa.html

[S49] C++：写文件
来源：http://hz.tianlin.xyz/gthdtgbnpu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tianlin.xyz/gtdhmdyzom.html

[S50] C++：格式化数字
来源：http://hz.hywenlv.cn/gtjhgitkuv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.kuanghao11.cn/gtmyrlbrsy.html

[S51] C++：显式类型转换
来源：http://hz.chenzaomai.com/gtalqtyvbn.html

static_cast<double>(a) / b
来源：http://hz.xziqi.cn/gtsnktaddl.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gtcajvaymj.html

int size() const noexcept { return n_; }
来源：http://hz.daxiang520.top/gtkldnzkfv.html

[S53] C++：移动语义
来源：http://hz.jqgfzy.top/gtehoezril.html

std::vector<int> w = std::move(v);
来源：http://hz.zycfv.cn/gtwltvyhip.html

[S54] C++：异常处理
来源：http://hz.jinqigufen.top/gtknxuxbco.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ydjk.org.cn/gttedgvony.html

[S55] C++：结构化绑定
来源：http://hz.ybcxt.top/gtccwnwfjb.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yueranfly.top/gtmgoycazo.html

[S56] C++：optional
来源：http://hz.zdqjudy.top/gtqopmvlck.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.havefunace.top/gtohtjzcbf.html

[S57] C++：编译期常量
来源：http://hz.xuetiantiany.cn/gtsdgvewpp.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtfeypmzgv.html

[S58] C++：命名空间
来源：http://hz.shanyushiyangtech.top/gtvrbnheeo.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtgqbumayq.html

[S59] C++：静态断言
来源：http://hz.zhiwuduotai.top/gternirwug.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.meibo888.top/gtxqsdpftk.html

[S60] C++：遍历并删除元素
来源：http://hz.svipenyu.cn/gtgeyzustj.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtjqxcmjor.html

================================================================================
来源：http://hz.hfpthk.cn/gtvyailpjn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zycfv.cn/gtyrmqvhnh.html

================================================================================
来源：http://hz.yangfankeji.com/gttsqlrral.html

[T01] Kotlin：Hello World
来源：http://hz.tian-w.cn/gtsnllknzk.html

println("Hello")
来源：http://hz.ivvv.top/gtjsqibnei.html

[T02] Kotlin：变量
来源：http://hz.ivvv.top/gtppatuysj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yj20258.top/gtbglszcrd.html

[T03] Kotlin：字符串模板
来源：http://hz.yj20258888.top/gtxjghfmoc.html

"值: $b"
来源：http://hz.jqgfzy.top/gtetrxwnrq.html

[T04] Kotlin：空安全
来源：http://hz.yvedp.cn/gthlgrbxlg.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtlrvhimiu.html

[T05] Kotlin：when 表达式
来源：http://hz.cheryme.top/gtfrpmoiub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.cheryme.top/gtgncarhla.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtcibocqkf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.shzxlz.cn/gtzozwcdfj.html

[T07] Kotlin：集合过滤
来源：http://hz.xylfe.cn/gthywgdtlf.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jlsjyb.cn/gtulotmyuh.html

[T08] Kotlin：数据类
来源：http://hz.yvedp.cn/gtwasfntdc.html

data class User(val name: String, val age: Int)
来源：http://hz.tianlin.xyz/gtmfeobgth.html

[T09] Kotlin：扩展函数
来源：http://hz.xingfuxueyuan.xyz/gtxbsgytqx.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtndlrpxwy.html

[T10] Kotlin：默认参数
来源：http://hz.andypj.xyz/gttllbkzug.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yangfankeji.com/gtcukmbdxu.html

[T11] Kotlin：协程
来源：http://hz.nanxuanxn.top/gtnocerpcn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gogol.net.cn/gtoyqwhsdx.html

[T12] Kotlin：解构声明
来源：http://hz.xuetiantiany.cn/gtgetitcya.html

val (a, b) = Pair(1, 2)
来源：http://hz.redwolf501.top/gtpyiyappe.html

[T13] Kotlin：只读 Map
来源：http://hz.xuetiantiany.cn/gtmhzwewew.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gtbpxpwmsz.html

[T14] Kotlin：循环
来源：http://hz.yongpay.top/gtdosnfefr.html

for (i in 1..10) println(i)
来源：http://hz.yuxming.cn/gtebkgzgvr.html

[T15] Kotlin：接口
来源：http://hz.9152youxi.cn/gtjoxhwrae.html

interface Shape { fun area(): Double }
来源：http://hz.sufxvd.cn/gtmldenewg.html

[T16] Swift：Hello World
来源：http://hz.hfpthk.cn/gtxkesbcoh.html

print("Hello")
来源：http://hz.redwolf501.top/gtrngjrpcm.html

[T17] Swift：变量与常量
来源：http://hz.ivvv.top/gtaxgtyjfn.html

var a = 1;  let b = 2
来源：http://hz.yuxming.cn/gtkiwpsjog.html

[T18] Swift：字符串插值
来源：http://hz.jinqigfzy.top/gtdpjoipec.html

"值: \(b)"
来源：http://hz.sweek.top/gtzsmadxfg.html

[T19] Swift：可选绑定
来源：http://hz.tianlin.xyz/gtepszuctd.html

if let n = opt { print(n) }
来源：http://hz.yonumen.top/gtrzdgiurv.html

[T20] Swift：数组操作
来源：http://hz.cheryme.top/gtssmcvjea.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhongyouzk.top/gtvmngzuym.html

[T21] Swift：遍历
来源：http://hz.hammf.cn/gtfpcuxgsd.html

for x in a { print(x) }
来源：http://hz.316326.xyz/gtvurzveoj.html

[T22] Swift：字典
来源：http://hz.yvedp.cn/gttrqbyxpt.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.cucudq.cn/gtfdlkyyme.html

[T23] Swift：函数
来源：http://hz.daria6918.cn/gtnevigjeh.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.cashguo.top/gtcaluuawr.html

[T24] Swift：闭包
来源：http://hz.xinyue.icu/gtxdubuzbd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.shanyushiyangkeji.top/gtmgtnmkrl.html

[T25] Swift：结构体
来源：http://hz.cqqwz.cn/gtxbbzdwhe.html

struct P { var x: Int }
来源：http://hz.zhijiandao.cn/gtvscmnwjm.html

[T26] Swift：类与重写
来源：http://hz.shanyushiyangkeji.top/gtmlsqigtd.html

class A: Base { override func f() {} }
来源：http://hz.quarkkingdee.top/gthqrdysnc.html

[T27] Swift：错误处理
来源：http://hz.cucudq.cn/gtvynjhfzd.html

do { try f() } catch { print(error) }
来源：http://hz.zhaomingkeji.xyz/gtrnxieroq.html

[T28] Swift：枚举
来源：http://hz.kuanghao11.cn/gtwshmsptw.html

enum Color { case red, green }
来源：http://hz.shuidangran.top/gtwajmuruk.html

[T29] Swift：guard 提前返回
来源：http://hz.quarkkingdee.top/gtryroials.html

guard let x = opt else { return }
来源：http://hz.jqgufenzy.top/gtycjojyvk.html

[T30] Swift：协议
来源：http://hz.yuanzhike.top/gtgqqnabij.html

protocol Shape { func area() -> Double }
来源：http://hz.redwolf501.top/gtuemcbhwf.html

[T31] Lua：Hello World
来源：http://hz.snrcjt.cn/gtiookpnkw.html

print("Hello")
来源：http://hz.svipenyu.cn/gtpjaftfhl.html

[T32] Lua：局部变量
来源：http://hz.hywenlv.cn/gtxwhuomku.html

local a = 1
来源：http://hz.yuxming.cn/gtoeuwemai.html


<!-- 参考信息 -->