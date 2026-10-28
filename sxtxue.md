代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jyoumei.cn/gtphxzmvjl.html

[R26] 命令替换
来源：http://hz.hnxiangtu.top/gtispbciei.html

now=$(date +%F); echo "$now"
来源：http://hz.andypj.xyz/gtxrogjrkq.html

[R27] 算术展开
来源：http://hz.cdnleiting.top/gtjiiqfamq.html

echo $((1 + 2 * 3))
来源：http://hz.yj20258.top/gtclvkuptv.html

[R28] 浮点运算
来源：http://hz.aizwys.cn/gtrkjhqbil.html

echo "scale=2; 10/3" | bc
来源：http://hz.yangfankeji.com/gtgiufcrvl.html

[R29] 定义函数
来源：http://hz.gogol.net.cn/gtjyffzvsp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xingfuxueyuan.xyz/gtkoattjhs.html

[R30] 函数返回状态码
来源：http://hz.cucudq.cn/gtdjjqxvrm.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhijiandao.cn/gtfjdtbfyi.html

[R31] 局部变量
来源：http://hz.cheryme.top/gthmawxryj.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gtgvyyzoge.html

[R32] 参数个数校验
来源：http://hz.ppjwa.cn/gthpsqpcoj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yongpay.top/gtjpnplulp.html

[R33] 捕获错误并提示行号
来源：http://hz.xinyue.icu/gtmqdgidcd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangkeji.top/gtcgostwls.html

[R34] 退出时清理
来源：http://hz.yj202588.top/gtjzfoutfc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenlongwang.top/gtvwdzrgsr.html

[R35] 后台执行并等待
来源：http://hz.yangfankeji.com/gtfulhsvjq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jinqigfzy.top/gtmebrkkkm.html

[R36] 并发执行多个任务
来源：http://hz.zhixingplan.top/gtlavrtdnz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hammf.cn/gtnsjolyqs.html

[R37] 把输出赋给变量
来源：http://hz.zhoulong.xyz/gttfzbynnz.html

files=$(ls -1)
来源：http://hz.shuidangran.top/gtbpnvyqjw.html

[R38] 管道串联
来源：http://hz.svipenyu.cn/gtuhavqjvp.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtwlybyhbr.html

[R39] 重定向标准输出与错误
来源：http://hz.zhoulong.xyz/gtobijpuqa.html

cmd > out.log 2>&1
来源：http://hz.tianlin.xyz/gttuhntquj.html

[R40] 追加写日志
来源：http://hz.9152youxi.cn/gtljnxckcd.html

echo "log" >> out.log
来源：http://hz.gzhubu.top/gttlrcmkfj.html

[R41] 丢弃输出
来源：http://hz.yvedp.cn/gtugcgcaqe.html

cmd >/dev/null 2>&1
来源：http://hz.shzxlz.cn/gtzrlbagto.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtgiqlnryl.html

wc -l < a.txt
来源：http://hz.quarkkingdee.top/gtlvreyjqt.html

[R43] 按名字查找文件
来源：http://hz.yvedp.cn/gtouyzipyt.html

find . -name "*.log" -type f
来源：http://hz.guannengcc.top/gtdtmapneh.html

[R44] 按修改时间查找
来源：http://hz.gotoacloud.top/gtzxjueckj.html

find . -mtime -7 -type f
来源：http://hz.zdqjudy.top/gtjkhwsewj.html

[R45] 批量删除
来源：http://hz.gzhubu.top/gtguuztlae.html

find . -name "*.tmp" -delete
来源：http://hz.hammf.cn/gtkogjdsaz.html

[R46] 递归替换文件内容
来源：http://hz.zycfv.cn/gtdiwhtvke.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gtunnwacoa.html

[R47] sed 单行替换
来源：http://hz.zhongyouzk.top/gtkzrtfetn.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zdqjudy.top/gtfwguqpxw.html

[R48] awk 取指定列
来源：http://hz.kuanghao11.cn/gtskbrcuot.html

awk '{print $1, $3}' a.txt
来源：http://hz.cdnleiting.top/gtshbqozdc.html

[R49] awk 带条件
来源：http://hz.yvedp.cn/gtkhfxsctx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.c1oappe.top/gtobyislmz.html

[R50] awk 求和
来源：http://hz.yangfankeji.com/gtjhbbpemz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtpuinjsjq.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gtuoyszdrz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.52xcode.cn/gtjfircbov.html

[R52] 统计行数
来源：http://hz.jiagoushi.top/gtrmdlsvll.html

wc -l a.txt
来源：http://hz.yvedp.cn/gttuxdagnk.html

[R53] 查看文件头与实时尾
来源：http://hz.chenlongwang.top/gtamfjaknd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hammf.cn/gttskxxfap.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtjckmaqek.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gtrsvxdpyz.html

[R55] 压缩与解压
来源：http://hz.zhongyouzk.top/gtmunwwkle.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gotoacloud.top/gttnshatot.html

[R56] 远程拷贝
来源：http://hz.hnqzz.top/gtqgoqlgug.html

scp file user@host:/path/
来源：http://hz.ivvv.top/gtkiuqdvrw.html

[R57] 远程执行命令
来源：http://hz.daria6918.cn/gtcsnioozq.html

ssh user@host 'uptime'
来源：http://hz.haohaochexian.top/gtlldyyzds.html

[R58] 下载文件
来源：http://hz.hnqzz.top/gtaiklever.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cucudq.cn/gtgbggoksz.html

[R59] 发 POST JSON
来源：http://hz.yj20258.top/gtlsioesai.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.wangdashe.top/gtkkhcrrwz.html

[R60] 只看 HTTP 状态码
来源：http://hz.ehwqpu.com/gtqxisleni.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yueranfly.top/gtwkhzdzpc.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtwbvksmfy.html

df -h;  du -sh *
来源：http://hz.shzxlz.cn/gtbkbzssev.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtxtrsdkvc.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtdvngfuhn.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtajabijyo.html

free -h;  ps aux | grep nginx
来源：http://hz.zhiwuduotai.top/gtyvftxsyw.html

[R64] 结束进程
来源：http://hz.chenjidiqi.icu/gtchinoigx.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yj20258.top/gtahhgyuue.html

[R65] 查看端口占用
来源：http://hz.pengpengdd.cyou/gtztajhzhz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guowangkeji.top/gtsnyudvmg.html

[R66] 定时任务
来源：http://hz.andypj.xyz/gtljmwldfc.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gttfbezrtx.html

[R67] 生成随机十六进制串
来源：http://hz.zycfv.cn/gtcpjssspc.html

openssl rand -hex 16
来源：http://hz.meibo888.top/gttyhpozmp.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtiwqetqaq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zdqjudy.top/gtodrnyvcb.html

[R69] 生成随机密码
来源：http://hz.ybcxt.top/gtynsfcvth.html

head -c 16 /dev/urandom | base64
来源：http://hz.ppjwa.cn/gtzuffkugz.html

[R70] 时间戳与互转
来源：http://hz.hnxiangtu.top/gtycmizonk.html

date +%s;  date -d @1700000000
来源：http://hz.svipenyu.cn/gtsucgzbpd.html

[R71] 日期格式化
来源：http://hz.cdnleiting.top/gtqnojikgn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.sufxvd.cn/gtplkhwqev.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtdpmvrryr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.mhx1999.top/gthpskybhg.html

[R73] 分割大日志
来源：http://hz.ydzc1.top/gtnwzrvezh.html

split -l 1000 big.log part_
来源：http://hz.yongpay.top/gtgjzrlvgg.html

[R74] 批量重命名
来源：http://hz.chenjidiqi.icu/gtipnguhjg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hywenlv.cn/gtdqmfqact.html

[R75] 导出环境变量
来源：http://hz.chenjidiqi.icu/gtuohvwmql.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ppjwa.cn/gteawizbpz.html

[R76] 使用临时文件
来源：http://hz.jianghu66.top/gtayxywkpd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtbtdgqiri.html

[R77] 读取用户输入
来源：http://hz.daria6918.cn/gtkwcbovts.html

read -rp "请输入: " ans
来源：http://hz.c1oappe.top/gtdrjkvtsb.html

[R78] 交互式菜单
来源：http://hz.yuxming.cn/gtsakevaur.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydjk.org.cn/gtkmraxjje.html

[R79] 解析命令行选项
来源：http://hz.xuetiantiany.cn/gtemxyicxq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zhoulong.xyz/gtfgtuccra.html

[R80] 查看脚本执行耗时
来源：http://hz.gzhubu.top/gtzkbvpbpk.html

time ./run.sh
来源：http://hz.0kj1m.cn/gtnoqcrnyg.html

================================================================================
来源：http://hz.chenlongwang.top/gtetztyilx.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtqgalypbw.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtxrlezizp.html

[S01] C：Hello World
来源：http://hz.zdqjudy.top/gtbfsnfklh.html

#include <stdio.h>
来源：http://hz.shangyingyoupin.top/gtpbmzfoac.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cashguo.top/gtmdyiznxu.html

[S02] C：变量与格式化输出
来源：http://hz.ybcxt.top/gtzborstkc.html

int a = 10; printf("%d\n", a);
来源：http://hz.wangdashe.top/gthdrxmnrz.html

[S03] C：读入整数
来源：http://hz.mhx1999.top/gthwmdiqwy.html

int x; scanf("%d", &x);
来源：http://hz.yuxming.cn/gtbvnbppsi.html

[S04] C：字符串复制
来源：http://hz.xingfuxueyuan.xyz/gtlddhkphn.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zycfv.cn/gtborrqooz.html

[S05] C：字符串长度
来源：http://hz.yongpay.top/gtnvhyrkhx.html

strlen(s)
来源：http://hz.gzhubu.top/gtuynvbzqe.html

[S06] C：字符串比较
来源：http://hz.shzxlz.cn/gtzadzaurc.html

strcmp(a, b) == 0
来源：http://hz.yuanzhike.top/gtopprovpy.html

[S07] C：数组遍历求和
来源：http://hz.hysaishi.cn/gtxnwpcysy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtroyxeqip.html

[S08] C：动态内存分配与释放
来源：http://hz.daria6918.cn/gtuclafvvz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.svipenyu.cn/gttiemerap.html

[S09] C：结构体定义与初始化
来源：http://hz.xingfuxueyuan.xyz/gtyrqwgsog.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhixingplan.top/gttclhcxpo.html

[S10] C：指针与解引用
来源：http://hz.feifeiyinyue.top/gtnofnfbmp.html

int *p = &a;  *p = 5;
来源：http://hz.9152youxi.cn/gtdtzuadyr.html

[S11] C：逐行读文件
来源：http://hz.jiagoushi.top/gtsqcdehpl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.tian-w.cn/gttpwkgzzw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jianghu66.top/gtynovongf.html

fclose(f);
来源：http://hz.xinyue.icu/gtwnltotmh.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtapfqersx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtbuvnszgl.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtrpqhjytd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xinyue.icu/gtaieeffqu.html

[S14] C：枚举
来源：http://hz.jiagoushi.top/gtforvdndf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.smart0.xyz/gtkwjwblkq.html

[S15] C：类型转换
来源：http://hz.pycfn.com/gtnqpdwowc.html

(double) a / b
来源：http://hz.redwolf501.top/gtmevyqlnc.html

[S16] C：位操作置位
来源：http://hz.jinqigfzy.top/gtyqrvxyiz.html

x |= (1 << 3);
来源：http://hz.tanke756.top/gtuvshonek.html

[S17] C：安全拼接字符串
来源：http://hz.yuanzhike.top/gtlndetytw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ehwqpu.com/gtougsdzwa.html

[S18] C：命令行参数
来源：http://hz.xingfuxueyuan.xyz/gtqrffyzzi.html

int main(int argc, char **argv)
来源：http://hz.iojbl.cn/gtrggrolzu.html

[S19] C：快速排序
来源：http://hz.svipenyu.cn/gtxkduwjoe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xingfuxueyuan.xyz/gtlfwyepom.html

[S20] C：二分查找
来源：http://hz.jqgufenzy.top/gtssuokquu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangkeji.top/gtvpnzfduc.html

[S21] C：字符类别判断
来源：http://hz.wangshuangyany.cn/gtzlnhmrif.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtokhcptsn.html

[S22] C：字符串转数字
来源：http://hz.jlsjyb.cn/gtdupqqlsl.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zdqjudy.top/gtriktaxiy.html

[S23] C：随机数
来源：http://hz.daria6918.cn/gtbmbmkjfe.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.meibo888.top/gtfsmroinu.html

[S24] C：获取本地时间
来源：http://hz.chenjidiqi.icu/gtxptzvnky.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daria6918.cn/gtleeydzih.html

[S25] C：内存拷贝
来源：http://hz.jiagoushi.top/gtczhtlgcw.html

memcpy(dst, src, n);
来源：http://hz.zhongyouzk.top/gtcybtmlzu.html

[S26] C：内存清零
来源：http://hz.pycfn.com/gtffxuvkuy.html

memset(a, 0, sizeof a);
来源：http://hz.hammf.cn/gtmzmpzuen.html

[S27] C：定义常量
来源：http://hz.hongshengwenyu.top/gthngcqkhb.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtvcttelvf.html

[S28] C：静态变量
来源：http://hz.hnxiangtu.top/gtwzsoqjzi.html

static int counter = 0;
来源：http://hz.cheryme.top/gtlrnzfyzh.html

[S29] C：变参函数
来源：http://hz.snrcjt.cn/gtwbblrmxu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.hfpthk.cn/gtrrxtulwr.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtdtbppuqp.html

#ifndef X_H
来源：http://hz.jianghu66.top/gttoqmxmrx.html

#define X_H
来源：http://hz.sxryk.cn/gtzaonriqe.html

#endif
来源：http://hz.sxryk.cn/gtbotpizgj.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtyhjnvtto.html

#include <iostream>
来源：http://hz.tian-w.cn/gtspqqqnwf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.smart0.xyz/gtncytczsi.html

[S32] C++：字符串
来源：http://hz.zycfv.cn/gtwlaeyddb.html

std::string s = "hi";  s += "!";
来源：http://hz.zhijiandao.cn/gtvpfulvxh.html

[S33] C++：vector 增删
来源：http://hz.9152youxi.cn/gtqwgllkbm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yanxiufei.cn/gteecwyost.html

[S34] C++：遍历 vector
来源：http://hz.svipenyu.cn/gtfhkjdsnb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jianghu66.top/gtvzciblpg.html

[S35] C++：map
来源：http://hz.jqgufenzy.top/gtdlngyopy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nanxuanxn.top/gtcwwrtoxx.html

[S36] C++：unordered_map
来源：http://hz.wangdashe.top/gtiadktfwl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shuidangran.top/gtbzajevqu.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtzhbqkmyz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zycfv.cn/gtxdktjztt.html

[S38] C++：排序
来源：http://hz.havefunace.top/gtibdybrhd.html

std::sort(v.begin(), v.end());
来源：http://hz.yuanzhike.top/gtxqyrzuzx.html

[S39] C++：自定义比较器排序
来源：http://hz.zhaomingkeji.xyz/gtlwpwiyff.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhiwuduotai.top/gtinknbxzl.html

[S40] C++：查找元素
来源：http://hz.birdmap.top/gtsnrtsqic.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yanxiufei.cn/gttukuhmrs.html

[S41] C++：类与构造函数
来源：http://hz.fengsongda.top/gtvoizoxmg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.svipenyu.cn/gtphsuspby.html

[S42] C++：继承与虚函数
来源：http://hz.guowangkeji.top/gtbijfvbvu.html

class B : public Base { public: void f() override {} };
来源：http://hz.jqgufenzy.top/gtrzwgexwm.html

[S43] C++：智能指针
来源：http://hz.nanxinkj.top/gtjtmfkgks.html

auto p = std::make_unique<int>(5);
来源：http://hz.quarkkingdee.top/gthyjnwtnn.html

[S44] C++：引用传参
来源：http://hz.andypj.xyz/gtdrxfyxhv.html

void inc(int &x) { ++x; }
来源：http://hz.xylfe.cn/gtiahrhtqk.html

[S45] C++：lambda
来源：http://hz.chenjidiqi.icu/gtmoewszxe.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gtxquivqij.html

[S46] C++：函数模板
来源：http://hz.chenjidiqi.icu/gtpejopofk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hnxiangtu.top/gtwyxrkacz.html

[S47] C++：结构化绑定遍历
来源：http://hz.sxryk.cn/gtsyfzvxqb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.kuanghao11.cn/gtoejjyspt.html

[S48] C++：逐行读文件
来源：http://hz.gaohongyu789.top/gthdudhhsn.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangkeji.top/gtatfomrlz.html

while (std::getline(in, line)) { }
来源：http://hz.iojbl.cn/gtxxqnnysq.html

[S49] C++：写文件
来源：http://hz.meibo888.top/gttycfivae.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tianlin.xyz/gtonrfzfcy.html

[S50] C++：格式化数字
来源：http://hz.pycfn.com/gtahinnutu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.jqgfzy.top/gtfmjifkfn.html

[S51] C++：显式类型转换
来源：http://hz.sweek.top/gtnajzimex.html

static_cast<double>(a) / b
来源：http://hz.guannengcc.top/gtkqgwlnpl.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gtjetcpzmk.html

int size() const noexcept { return n_; }
来源：http://hz.ydjk.org.cn/gttecugipb.html

[S53] C++：移动语义
来源：http://hz.kuanghao11.cn/gtlowfkqbs.html

std::vector<int> w = std::move(v);
来源：http://hz.hammf.cn/gtsndgutjs.html

[S54] C++：异常处理
来源：http://hz.quarkkingdee.top/gtyrheabvl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yj20258.top/gtwuaapwez.html

[S55] C++：结构化绑定
来源：http://hz.hywenlv.cn/gtbclbsgmv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ydjk.org.cn/gtudttaekd.html

[S56] C++：optional
来源：http://hz.havefunace.top/gtjgfanwnt.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.cqqwz.cn/gtwqvajozy.html

[S57] C++：编译期常量
来源：http://hz.zhengqikj.top/gtyjmogszs.html

constexpr int N = 10;
来源：http://hz.haohaochexian.top/gtdyqzkrss.html

[S58] C++：命名空间
来源：http://hz.aibaodan.cn/gtblwjfymo.html

namespace ns { int f() { return 1; } }
来源：http://hz.zhiwuduotai.top/gtdspuscle.html

[S59] C++：静态断言
来源：http://hz.hfpthk.cn/gtimykgcmf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.havefunace.top/gtafceeknt.html

[S60] C++：遍历并删除元素
来源：http://hz.xuetiantiany.cn/gtnekcncbs.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.mhx1999.top/gtrqhisbhk.html

================================================================================
来源：http://hz.ehwqpu.com/gtzobhicon.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nanxuanxn.top/gtlcqtdcbb.html

================================================================================
来源：http://hz.sufxvd.cn/gtrzsbsvql.html

[T01] Kotlin：Hello World
来源：http://hz.0kj1m.cn/gtqqreuoui.html

println("Hello")
来源：http://hz.yj20258.top/gtqmyoabhw.html

[T02] Kotlin：变量
来源：http://hz.fengsongda.top/gtepjvnjjj.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhixingplan.top/gtkfwfbusc.html

[T03] Kotlin：字符串模板
来源：http://hz.yonumen.top/gtwjdndwiy.html

"值: $b"
来源：http://hz.hfpthk.cn/gtnrshiasv.html

[T04] Kotlin：空安全
来源：http://hz.0kj1m.cn/gtgdrqecty.html

val n: String? = null;  n?.length
来源：http://hz.mhx1999.top/gtgnpqujwl.html

[T05] Kotlin：when 表达式
来源：http://hz.zhiwuduotai.top/gtmlemnzdk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ywan-chungtsiang.top/gtbupgepxb.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gtqonubhad.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.aibaodan.cn/gtrnbssabd.html

[T07] Kotlin：集合过滤
来源：http://hz.xylfe.cn/gtuappmtme.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ppjwa.cn/gtqqmiyxnl.html

[T08] Kotlin：数据类
来源：http://hz.dashuyun.cn/gtxnenndic.html

data class User(val name: String, val age: Int)
来源：http://hz.cdnleiting.top/gtdojnllaj.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gttljrxzms.html

fun String.exclaim() = this + "!"
来源：http://hz.sufxvd.cn/gtjawrscdr.html

[T10] Kotlin：默认参数
来源：http://hz.pycfn.com/gtpfcwlqoa.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.shangyingyoupin.top/gtozqqujxy.html

[T11] Kotlin：协程
来源：http://hz.gotoacloud.top/gtiogbaehm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.sufxvd.cn/gtaurbakzb.html

[T12] Kotlin：解构声明
来源：http://hz.daxiang520.top/gtxydudvva.html

val (a, b) = Pair(1, 2)
来源：http://hz.cheryme.top/gtivyomicm.html

[T13] Kotlin：只读 Map
来源：http://hz.shzxlz.cn/gtlgndavkq.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gtbtcyvzdo.html

[T14] Kotlin：循环
来源：http://hz.yuanzhike.top/gtvdpglaiv.html

for (i in 1..10) println(i)
来源：http://hz.fzhhl.top/gtauqzgiix.html

[T15] Kotlin：接口
来源：http://hz.jianghu66.top/gtosfzqfet.html

interface Shape { fun area(): Double }
来源：http://hz.xuanzx.com/gtkjghzytb.html

[T16] Swift：Hello World
来源：http://hz.zhaomingkeji.xyz/gtdxnkptrh.html

print("Hello")
来源：http://hz.guowangkeji.top/gtxnryfdlh.html

[T17] Swift：变量与常量
来源：http://hz.xylfe.cn/gtvtlspqrc.html

var a = 1;  let b = 2
来源：http://hz.kuanghao11.cn/gtyqivrvcx.html

[T18] Swift：字符串插值
来源：http://hz.jqgfzy.top/gtaylgfhdn.html

"值: \(b)"
来源：http://hz.xingfuxueyuan.xyz/gtynulozay.html

[T19] Swift：可选绑定
来源：http://hz.sufxvd.cn/gtilfhnxkw.html

if let n = opt { print(n) }
来源：http://hz.andypj.xyz/gtcaenwcpr.html

[T20] Swift：数组操作
来源：http://hz.9152youxi.cn/gtqfqjqycg.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhongyouzk.top/gtvlkxdjjn.html

[T21] Swift：遍历
来源：http://hz.ybcxt.top/gtoirwjszq.html

for x in a { print(x) }
来源：http://hz.pycfn.com/gteogaymee.html

[T22] Swift：字典
来源：http://hz.guannengcc.top/gtxpqhnkbz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ybcxt.top/gtgfqkyhzw.html

[T23] Swift：函数
来源：http://hz.316326.xyz/gtlfoavcea.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hywenlv.cn/gtedleopms.html

[T24] Swift：闭包
来源：http://hz.vqdsnc.cn/gtegnkmnzw.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.jinyuanbaomall.cn/gtvwkixoho.html

[T25] Swift：结构体
来源：http://hz.tian-w.cn/gtjsrugsbr.html

struct P { var x: Int }
来源：http://hz.yonumen.top/gtmxonmcfv.html

[T26] Swift：类与重写
来源：http://hz.hnxiangtu.top/gtfhkzwbhs.html

class A: Base { override func f() {} }
来源：http://hz.yongpay.top/gtzkevxwhm.html

[T27] Swift：错误处理
来源：http://hz.yj202588.top/gtnppqwaiq.html

do { try f() } catch { print(error) }
来源：http://hz.guannengcc.top/gtdwssaazq.html

[T28] Swift：枚举
来源：http://hz.hongshengwenyu.top/gtzrddduzv.html

enum Color { case red, green }
来源：http://hz.birdmap.top/gtfzcbpfyj.html


<!-- 参考信息 -->