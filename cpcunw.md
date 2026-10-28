代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhiwuduotai.top/gtdlmzrnnb.html

[R24] 大小写转换
来源：http://hz.ivvv.top/gtdytukjcy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhijiandao.cn/gtymonroid.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtmksmyuha.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.havefunace.top/gtqpgnhnhx.html

[R26] 命令替换
来源：http://hz.52xcode.cn/gtlybuqjsg.html

now=$(date +%F); echo "$now"
来源：http://hz.birdmap.top/gtdhwlirtr.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gtfsoctkgb.html

echo $((1 + 2 * 3))
来源：http://hz.jiagoushi.top/gtzawahctc.html

[R28] 浮点运算
来源：http://hz.ehwqpu.com/gtmmvqquza.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtsercyaor.html

[R29] 定义函数
来源：http://hz.zhengqikj.top/gtghipencr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.cheryme.top/gtgdivtvqc.html

[R30] 函数返回状态码
来源：http://hz.yj20258888.top/gtfcqzhpkv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ywan-chungtsiang.top/gtjcvmdfud.html

[R31] 局部变量
来源：http://hz.ydjk.org.cn/gtpgvvufug.html

f() { local x=1; echo "$x"; }
来源：http://hz.cucudq.cn/gtijammlpi.html

[R32] 参数个数校验
来源：http://hz.redwolf501.top/gtnragenzr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jiagoushi.top/gtctfycfgp.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtdswgmkwm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.nanxuanxn.top/gtbfercpfw.html

[R34] 退出时清理
来源：http://hz.quarkkingdee.top/gtyrfcgkca.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.chenjidiqi.icu/gtklcaxbuf.html

[R35] 后台执行并等待
来源：http://hz.snrcjt.cn/gtgzaekzvd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yueranfly.top/gtpiueklqr.html

[R36] 并发执行多个任务
来源：http://hz.dianchejie.cn/gtiprminef.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nwbrower.top/gtrfvhknay.html

[R37] 把输出赋给变量
来源：http://hz.shanyushiyangtech.top/gtqshljrus.html

files=$(ls -1)
来源：http://hz.gogol.net.cn/gtybwmvydc.html

[R38] 管道串联
来源：http://hz.shanyushiyangkeji.top/gtbitsqple.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daxiang520.top/gtykutmifv.html

[R39] 重定向标准输出与错误
来源：http://hz.fengsongda.top/gtddtmyuhj.html

cmd > out.log 2>&1
来源：http://hz.zhengqikj.top/gtcvrkqesv.html

[R40] 追加写日志
来源：http://hz.jqgufenzy.top/gtryxcdqzn.html

echo "log" >> out.log
来源：http://hz.jinqigfzy.top/gtfgocdegi.html

[R41] 丢弃输出
来源：http://hz.nanxinkj.top/gthzhflmhn.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtfyqdlwqs.html

[R42] 输入重定向
来源：http://hz.wangshuangyany.cn/gtczcxjqst.html

wc -l < a.txt
来源：http://hz.meibo888.top/gtfrkkkxpm.html

[R43] 按名字查找文件
来源：http://hz.hywenlv.cn/gttledqpkn.html

find . -name "*.log" -type f
来源：http://hz.xuetiantiany.cn/gtghdpkniv.html

[R44] 按修改时间查找
来源：http://hz.shangyingyoupin.top/gtvmlmwhvv.html

find . -mtime -7 -type f
来源：http://hz.ivvv.top/gtsytbmaea.html

[R45] 批量删除
来源：http://hz.daria6918.cn/gtskrkqaib.html

find . -name "*.tmp" -delete
来源：http://hz.316326.xyz/gtfdgkmxcu.html

[R46] 递归替换文件内容
来源：http://hz.dianchejie.cn/gtnsxiyulr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ppjwa.cn/gttmdakyqz.html

[R47] sed 单行替换
来源：http://hz.yuanzhike.top/gtnqxfvoav.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yvedp.cn/gtslnhopzn.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gtfbthpcmi.html

awk '{print $1, $3}' a.txt
来源：http://hz.gaohongyu789.top/gtpcwennxd.html

[R49] awk 带条件
来源：http://hz.jiagoushi.top/gtqndzumzn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.feifeiyinyue.top/gtgqueqyej.html

[R50] awk 求和
来源：http://hz.shuidangran.top/gtsqdquknm.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ywan-chungtsiang.top/gtofixlauh.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtqekefooi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hongshengwenyu.top/gtiqybkzlc.html

[R52] 统计行数
来源：http://hz.nanxuanxn.top/gtpxknblkj.html

wc -l a.txt
来源：http://hz.haohaochexian.top/gtwgapeilx.html

[R53] 查看文件头与实时尾
来源：http://hz.yuanzhike.top/gthfwnxatc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hnqzz.top/gtqtcohbwu.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangtech.top/gtbxcowyig.html

diff a.txt b.txt
来源：http://hz.jqgfzy.top/gtckqysnjt.html

[R55] 压缩与解压
来源：http://hz.jinghuilouyu.cn/gtbmkywjsn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yj20258.top/gteadpwvaa.html

[R56] 远程拷贝
来源：http://hz.tianlin.xyz/gtmyachmke.html

scp file user@host:/path/
来源：http://hz.zhaomingkeji.xyz/gthkxjhjzf.html

[R57] 远程执行命令
来源：http://hz.cashguo.top/gtwsrzvafb.html

ssh user@host 'uptime'
来源：http://hz.ywan-chungtsiang.top/gtnyyxqsaz.html

[R58] 下载文件
来源：http://hz.zhengqikj.top/gtbilplwuq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuanzx.com/gtyjqhwzgd.html

[R59] 发 POST JSON
来源：http://hz.xinyue.icu/gtyduyzguv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yanxiufei.cn/gtgjplopjp.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gtrujuycwt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.smart0.xyz/gtlrzudbfm.html

[R61] 磁盘占用
来源：http://hz.gaohongyu789.top/gtveddzpkm.html

df -h;  du -sh *
来源：http://hz.gaohongyu789.top/gtbvcpxqug.html

[R62] 找最占空间的文件
来源：http://hz.cucudq.cn/gtrujijgdi.html

du -ah . | sort -rh | head -10
来源：http://hz.hysaishi.cn/gtchguanww.html

[R63] 内存与进程
来源：http://hz.hywenlv.cn/gtsaudcyta.html

free -h;  ps aux | grep nginx
来源：http://hz.52xcode.cn/gtdhjyqlex.html

[R64] 结束进程
来源：http://hz.mhx1999.top/gtbyaxsymy.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yongpay.top/gtsizavakx.html

[R65] 查看端口占用
来源：http://hz.havefunace.top/gtfntckyzy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gteyojrsyg.html

[R66] 定时任务
来源：http://hz.mhx1999.top/gtmhtnizmz.html

crontab -e;  crontab -l
来源：http://hz.redwolf501.top/gtsixonfdi.html

[R67] 生成随机十六进制串
来源：http://hz.yj202588.top/gtfqxoscdr.html

openssl rand -hex 16
来源：http://hz.jinghuilouyu.cn/gtaqodiryq.html

[R68] 计算文件校验值
来源：http://hz.jinyuanbaomall.cn/gtboefrcsq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.52xcode.cn/gtewwfkwoq.html

[R69] 生成随机密码
来源：http://hz.pengpengdd.cyou/gtfdfmvwkb.html

head -c 16 /dev/urandom | base64
来源：http://hz.feifeiyinyue.top/gtjeizwuzq.html

[R70] 时间戳与互转
来源：http://hz.cucudq.cn/gtnmxcjehs.html

date +%s;  date -d @1700000000
来源：http://hz.zhiwuduotai.top/gttyilhejc.html

[R71] 日期格式化
来源：http://hz.jqgufenzy.top/gtifasvocl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtbjujxrpq.html

[R72] 等待端口就绪
来源：http://hz.fzhhl.top/gtvmjphcdd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nanxuanxn.top/gtqfdguuuz.html

[R73] 分割大日志
来源：http://hz.jlsjyb.cn/gtfbdjwyfa.html

split -l 1000 big.log part_
来源：http://hz.meibo888.top/gtjersvmbt.html

[R74] 批量重命名
来源：http://hz.cqqwz.cn/gtlpxpjqja.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.tian-w.cn/gtxeckiohi.html

[R75] 导出环境变量
来源：http://hz.zhiwuduotai.top/gtdensnzzg.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shangyingyoupin.top/gtqywikhum.html

[R76] 使用临时文件
来源：http://hz.9152youxi.cn/gtehwwwmvd.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtbhaidgfv.html

[R77] 读取用户输入
来源：http://hz.jiagoushi.top/gtujlgkvxm.html

read -rp "请输入: " ans
来源：http://hz.zhoulong.xyz/gtzhwehtrj.html

[R78] 交互式菜单
来源：http://hz.hnqzz.top/gtzugmsgbi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.0kj1m.cn/gtzgrlxyjy.html

[R79] 解析命令行选项
来源：http://hz.nanxinkj.top/gtfmlsoaiz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cucudq.cn/gtwarkmdty.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gtvjxqkumj.html

time ./run.sh
来源：http://hz.redwolf501.top/gtuwhelbhc.html

================================================================================
来源：http://hz.ppjwa.cn/gtsphsacjc.html

S. C / C++ 专题
来源：http://hz.yonumen.top/gtvtmzbctf.html

================================================================================
来源：http://hz.hnqzz.top/gtocqjtkkb.html

[S01] C：Hello World
来源：http://hz.daria6918.cn/gtphznatzh.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtvrvpvdqo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtfkizsead.html

[S02] C：变量与格式化输出
来源：http://hz.snrcjt.cn/gtfimvsdon.html

int a = 10; printf("%d\n", a);
来源：http://hz.yj20258.top/gtltayfuyo.html

[S03] C：读入整数
来源：http://hz.cqqwz.cn/gtwpsvpnqe.html

int x; scanf("%d", &x);
来源：http://hz.tanke756.top/gtnpdrgpni.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtgpjzjupv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.nanxuanxn.top/gthduwwnub.html

[S05] C：字符串长度
来源：http://hz.dashuyun.cn/gttbtveuwd.html

strlen(s)
来源：http://hz.cqqwz.cn/gtlxctyxar.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gthpewlvpg.html

strcmp(a, b) == 0
来源：http://hz.ivvv.top/gtzfwmtkkm.html

[S07] C：数组遍历求和
来源：http://hz.yangfankeji.com/gtjohknjyh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.52xcode.cn/gtzgdzgavt.html

[S08] C：动态内存分配与释放
来源：http://hz.zhongyouzk.top/gtouaulklp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtpdedwptb.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtigmtjtjf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtimlpfuor.html

[S10] C：指针与解引用
来源：http://hz.chenzaomai.com/gtmhnfhtux.html

int *p = &a;  *p = 5;
来源：http://hz.c1oappe.top/gttcndkahw.html

[S11] C：逐行读文件
来源：http://hz.chenjidiqi.icu/gteiurrlcr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.bjfxy.top/gtdzbldaoh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yonumen.top/gtckmaemcw.html

fclose(f);
来源：http://hz.zhoulong.xyz/gtghpvepho.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtlywuhoty.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.pengpengdd.cyou/gtsxhprtrg.html

[S13] C：宏定义
来源：http://hz.zhaomingkeji.xyz/gthqftvvhx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenjidiqi.icu/gtfdpyiedd.html

[S14] C：枚举
来源：http://hz.ehwqpu.com/gtfuobqzqf.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yueranfly.top/gtqaajsenz.html

[S15] C：类型转换
来源：http://hz.xziqi.cn/gtvfmxljhm.html

(double) a / b
来源：http://hz.hongshengwenyu.top/gtyvbnblox.html

[S16] C：位操作置位
来源：http://hz.316326.xyz/gtllqdvwxp.html

x |= (1 << 3);
来源：http://hz.jiagoushi.top/gtcxjwqeuo.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigufen.top/gtcgfwmltk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.kuanghao11.cn/gtyqicjiqy.html

[S18] C：命令行参数
来源：http://hz.xuetiantiany.cn/gtuomulrki.html

int main(int argc, char **argv)
来源：http://hz.yuanzhike.top/gtcstkghia.html

[S19] C：快速排序
来源：http://hz.yj20258888.top/gtmqxzgpwe.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gtmkupdmrk.html

[S20] C：二分查找
来源：http://hz.daria6918.cn/gtdvppuqfc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gthnqqiiso.html

[S21] C：字符类别判断
来源：http://hz.xylfe.cn/gtkfwkvrkx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxinkj.top/gtuffykzon.html

[S22] C：字符串转数字
来源：http://hz.hnqzz.top/gtlkmurvnc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.daxiang520.top/gtnbpyxixl.html

[S23] C：随机数
来源：http://hz.hysaishi.cn/gtrwuryefk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.c1oappe.top/gtuvcoznhz.html

[S24] C：获取本地时间
来源：http://hz.yongpay.top/gtnhnlavkb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yonumen.top/gtlddijovi.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtfferyiue.html

memcpy(dst, src, n);
来源：http://hz.fzhhl.top/gtuxorxbuj.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtjmcnydzl.html

memset(a, 0, sizeof a);
来源：http://hz.cqqwz.cn/gtpzsiosgd.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtovwssdun.html

const double PI = 3.14159;
来源：http://hz.zhijiandao.cn/gthqkavfbn.html

[S28] C：静态变量
来源：http://hz.yanxiufei.cn/gtplcoborr.html

static int counter = 0;
来源：http://hz.hywenlv.cn/gtwihxofan.html

[S29] C：变参函数
来源：http://hz.cucudq.cn/gtkkdzsptz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.dianchejie.cn/gthbcghxmf.html

[S30] C：头文件保护
来源：http://hz.hongshengwenyu.top/gtakjsnicz.html

#ifndef X_H
来源：http://hz.feifeiyinyue.top/gtfladexuk.html

#define X_H
来源：http://hz.smart0.xyz/gtnrmtnldk.html

#endif
来源：http://hz.guowangkeji.top/gtpqbofbtj.html

[S31] C++：Hello World
来源：http://hz.xuetiantiany.cn/gtcxgzbvlz.html

#include <iostream>
来源：http://hz.hongshengwenyu.top/gtodbuyqji.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.0kj1m.cn/gtwmpbadvi.html

[S32] C++：字符串
来源：http://hz.hywenlv.cn/gtjkzyfnbr.html

std::string s = "hi";  s += "!";
来源：http://hz.iojbl.cn/gtsmurryrb.html

[S33] C++：vector 增删
来源：http://hz.pycfn.com/gtsxhrszgm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.316326.xyz/gtrnplymar.html

[S34] C++：遍历 vector
来源：http://hz.316326.xyz/gtbwpirtjv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ywan-chungtsiang.top/gtjqqaaomj.html

[S35] C++：map
来源：http://hz.chenjidiqi.icu/gtnuujsfqk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gtbhwlvysm.html

[S36] C++：unordered_map
来源：http://hz.redwolf501.top/gtjojusbxf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.daxiang520.top/gtkvfmrzri.html

[S37] C++：set
来源：http://hz.xuetiantiany.cn/gttfbvyass.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.pengpengdd.cyou/gtimjtaatg.html

[S38] C++：排序
来源：http://hz.mhx1999.top/gtbslvjfut.html

std::sort(v.begin(), v.end());
来源：http://hz.gaohongyu789.top/gtrqnijrfk.html

[S39] C++：自定义比较器排序
来源：http://hz.fengsongda.top/gtqcllrjoq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtuyhzqvzz.html

[S40] C++：查找元素
来源：http://hz.guannengcc.top/gtdocgtiac.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jinghuilouyu.cn/gtckgjmkix.html

[S41] C++：类与构造函数
来源：http://hz.jlsjyb.cn/gthxjjcogv.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xziqi.cn/gtqbzfmcjr.html

[S42] C++：继承与虚函数
来源：http://hz.daxiang520.top/gtddzmibft.html

class B : public Base { public: void f() override {} };
来源：http://hz.iojbl.cn/gtbnntemhq.html

[S43] C++：智能指针
来源：http://hz.ywan-chungtsiang.top/gtblklmvzs.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuanzhike.top/gtgiquxonl.html

[S44] C++：引用传参
来源：http://hz.jqgufenzy.top/gtahsdahud.html

void inc(int &x) { ++x; }
来源：http://hz.hywenlv.cn/gteupubend.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtwdntsuzw.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.snrcjt.cn/gtkqxlmtya.html

[S46] C++：函数模板
来源：http://hz.dianchejie.cn/gtdpsyoyhg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ivvv.top/gtcpdxqgjg.html

[S47] C++：结构化绑定遍历
来源：http://hz.chenjidiqi.icu/gthnuewmra.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hammf.cn/gtcmycambt.html

[S48] C++：逐行读文件
来源：http://hz.redwolf501.top/gtkekvgvvf.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yuxming.cn/gtrsarvdxh.html

while (std::getline(in, line)) { }
来源：http://hz.nwbrower.top/gtvyzcgiei.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gtkkfmjuuv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.shanyushiyangtech.top/gtsupsvywi.html

[S50] C++：格式化数字
来源：http://hz.zhongyouzk.top/gtqhmwpqpc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenlongwang.top/gtvbgfcdaq.html

[S51] C++：显式类型转换
来源：http://hz.hysaishi.cn/gtvkjeanxb.html

static_cast<double>(a) / b
来源：http://hz.birdmap.top/gtoiuqaxni.html

[S52] C++：const 与 noexcept
来源：http://hz.jqgufenzy.top/gtalagkamj.html

int size() const noexcept { return n_; }
来源：http://hz.yuanzhike.top/gtkxmlquhc.html

[S53] C++：移动语义
来源：http://hz.jinyuanbaomall.cn/gtbqpqngvi.html

std::vector<int> w = std::move(v);
来源：http://hz.zhixingplan.top/gtgwfikkzr.html

[S54] C++：异常处理
来源：http://hz.gogol.net.cn/gtydjqvlet.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhengqikj.top/gtefvasphg.html

[S55] C++：结构化绑定
来源：http://hz.ydzc1.top/gtcpuoujhf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zdqjudy.top/gtwbhsfgau.html

[S56] C++：optional
来源：http://hz.xuanzx.com/gtszdsfklg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tianlin.xyz/gtwwwggqmb.html

[S57] C++：编译期常量
来源：http://hz.iojbl.cn/gtrmynsbgo.html

constexpr int N = 10;
来源：http://hz.jqgufenzy.top/gtolrvywtd.html

[S58] C++：命名空间
来源：http://hz.nwbrower.top/gthfuwkdog.html

namespace ns { int f() { return 1; } }
来源：http://hz.ywan-chungtsiang.top/gtqzgnoahs.html

[S59] C++：静态断言
来源：http://hz.tianlin.xyz/gtohedjmxb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.redwolf501.top/gtkcqrhzyj.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gttharxdhu.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.hammf.cn/gtkkllsdke.html

================================================================================
来源：http://hz.zdqjudy.top/gtnwqitpda.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.hnxiangtu.top/gtrszpfxrk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtsngjgwxx.html

[T01] Kotlin：Hello World
来源：http://hz.snrcjt.cn/gtcdxzggdn.html

println("Hello")
来源：http://hz.birdmap.top/gtudhkbgew.html

[T02] Kotlin：变量
来源：http://hz.zhengqikj.top/gtobdpormd.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.jinqigfzy.top/gtorchnuwq.html

[T03] Kotlin：字符串模板
来源：http://hz.jinyuanbaomall.cn/gtnpxnrfxz.html

"值: $b"
来源：http://hz.jinghuilouyu.cn/gtrgsodhlx.html

[T04] Kotlin：空安全
来源：http://hz.hysaishi.cn/gttuqygncw.html

val n: String? = null;  n?.length
来源：http://hz.shangyingyoupin.top/gtklwkodgq.html

[T05] Kotlin：when 表达式
来源：http://hz.mhx1999.top/gtlnaaftki.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.ywan-chungtsiang.top/gtwzudmobo.html

[T06] Kotlin：集合映射
来源：http://hz.tian-w.cn/gtfiggbrzq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhongyouzk.top/gtkvwkvftr.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtfmcwgzkb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtrxxerfrq.html

[T08] Kotlin：数据类
来源：http://hz.meibo888.top/gtxmcjjwop.html

data class User(val name: String, val age: Int)
来源：http://hz.gotoacloud.top/gtjfzzuuuv.html

[T09] Kotlin：扩展函数
来源：http://hz.vqdsnc.cn/gtciijbfxn.html

fun String.exclaim() = this + "!"
来源：http://hz.sweek.top/gtfewommgz.html

[T10] Kotlin：默认参数
来源：http://hz.zycfv.cn/gtrwhgevha.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtgmwzmnay.html

[T11] Kotlin：协程
来源：http://hz.xuanzx.com/gtszpyuemn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtvwvtqung.html

[T12] Kotlin：解构声明
来源：http://hz.meibo888.top/gtuwipzqem.html

val (a, b) = Pair(1, 2)
来源：http://hz.guowangkeji.top/gtcsiszfhj.html

[T13] Kotlin：只读 Map
来源：http://hz.nanxuanxn.top/gtyiocbtoo.html

val m = mapOf("a" to 1)
来源：http://hz.jianghu66.top/gtwcwkvtkb.html

[T14] Kotlin：循环
来源：http://hz.52xcode.cn/gtkawagkyz.html

for (i in 1..10) println(i)
来源：http://hz.chenlongwang.top/gtohvzugsz.html

[T15] Kotlin：接口
来源：http://hz.fzhhl.top/gtwdvvyxjr.html

interface Shape { fun area(): Double }
来源：http://hz.hfpthk.cn/gtvkzvlxdt.html

[T16] Swift：Hello World
来源：http://hz.yj20258888.top/gtnyrqnypr.html

print("Hello")
来源：http://hz.vqdsnc.cn/gtpaaqlhth.html

[T17] Swift：变量与常量
来源：http://hz.gaohongyu789.top/gtpashfcms.html

var a = 1;  let b = 2
来源：http://hz.vqdsnc.cn/gtimtdlkss.html

[T18] Swift：字符串插值
来源：http://hz.yueranfly.top/gtsotzojwn.html

"值: \(b)"
来源：http://hz.zycfv.cn/gttezwyiqw.html

[T19] Swift：可选绑定
来源：http://hz.316326.xyz/gtiefipzvz.html

if let n = opt { print(n) }
来源：http://hz.yongpay.top/gtgoozbytz.html

[T20] Swift：数组操作
来源：http://hz.xinyue.icu/gtzqrqhbvy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.hnqzz.top/gtqddotcih.html

[T21] Swift：遍历
来源：http://hz.yangfankeji.com/gtngstwqdd.html

for x in a { print(x) }
来源：http://hz.nanxuanxn.top/gtnnaqrxje.html

[T22] Swift：字典
来源：http://hz.havefunace.top/gtlutjicsk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.zhijiandao.cn/gtxulgvmeg.html

[T23] Swift：函数
来源：http://hz.shanyushiyangkeji.top/gtcwnfobkr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.yueranfly.top/gtogpdiwby.html

[T24] Swift：闭包
来源：http://hz.chenzaomai.com/gtuuhhigiv.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.gzhubu.top/gtrzuetkrv.html

[T25] Swift：结构体
来源：http://hz.52xcode.cn/gtfraelpve.html

struct P { var x: Int }
来源：http://hz.yanxiufei.cn/gtdpgrwabr.html

[T26] Swift：类与重写
来源：http://hz.tanke756.top/gtzbhxonce.html

class A: Base { override func f() {} }
来源：http://hz.havefunace.top/gthuupzyzh.html


<!-- 参考信息 -->