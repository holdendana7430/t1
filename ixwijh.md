代发 wailian999

echo "${#s}"
来源：http://hz.shzxlz.cn/gtqbnlrhms.html

[R22] 截取子串
来源：http://hz.ywan-chungtsiang.top/gtfjhuszgy.html

echo "${s:0:5}"
来源：http://hz.yj20258.top/gtryjqnbth.html

[R23] 字符串替换
来源：http://hz.pycfn.com/gtkgcgrcli.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.svipenyu.cn/gtgahjgkii.html

[R24] 大小写转换
来源：http://hz.cqqwz.cn/gtrzcieisi.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gtulacxivb.html

[R25] 去后缀 / 去前缀
来源：http://hz.daria6918.cn/gtfzkceflv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yongpay.top/gtubwbnxqn.html

[R26] 命令替换
来源：http://hz.c1oappe.top/gtqyvwnflh.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigufen.top/gtrnjygtkr.html

[R27] 算术展开
来源：http://hz.gogol.net.cn/gtjsffvjmi.html

echo $((1 + 2 * 3))
来源：http://hz.yangfankeji.com/gtypumkiac.html

[R28] 浮点运算
来源：http://hz.jianghu66.top/gtcppyminh.html

echo "scale=2; 10/3" | bc
来源：http://hz.vqdsnc.cn/gtybhynfcn.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gtaescngdp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gtxyimgaij.html

[R30] 函数返回状态码
来源：http://hz.chenlongwang.top/gttaifchba.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.nanxuanxn.top/gtlzkejusp.html

[R31] 局部变量
来源：http://hz.haohaochexian.top/gtziwejaht.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gteekmrpyb.html

[R32] 参数个数校验
来源：http://hz.xylfe.cn/gtzpyhdibh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.gogol.net.cn/gtuwcndnkc.html

[R33] 捕获错误并提示行号
来源：http://hz.jinyuanbaomall.cn/gthiwmfzpr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhijiandao.cn/gtispkjkdd.html

[R34] 退出时清理
来源：http://hz.shuidangran.top/gtodwgubxq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hysaishi.cn/gtzgzsawei.html

[R35] 后台执行并等待
来源：http://hz.chenzaomai.com/gtgaklhgwy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.sxryk.cn/gtjyklpkjv.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtxjezvadd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gteoybzgbk.html

[R37] 把输出赋给变量
来源：http://hz.yuanzhike.top/gtotbcatvi.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtedykevty.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gtetitlwfa.html

cat a.txt | grep -i error | wc -l
来源：http://hz.aibaodan.cn/gtwexxfxuq.html

[R39] 重定向标准输出与错误
来源：http://hz.smart0.xyz/gtajgruyxf.html

cmd > out.log 2>&1
来源：http://hz.hnqzz.top/gtfulzlqun.html

[R40] 追加写日志
来源：http://hz.yj20258888.top/gtdbqlayvy.html

echo "log" >> out.log
来源：http://hz.xinyue.icu/gtuuxstpoz.html

[R41] 丢弃输出
来源：http://hz.haohaochexian.top/gtcwqktksp.html

cmd >/dev/null 2>&1
来源：http://hz.xuetiantiany.cn/gteubhwdct.html

[R42] 输入重定向
来源：http://hz.yanxiufei.cn/gtngmyutdg.html

wc -l < a.txt
来源：http://hz.shanyushiyangkeji.top/gtjoyhwwev.html

[R43] 按名字查找文件
来源：http://hz.gotoacloud.top/gtchwpyqzc.html

find . -name "*.log" -type f
来源：http://hz.sweek.top/gtqbufhjpz.html

[R44] 按修改时间查找
来源：http://hz.zhixingplan.top/gtzrlpwcyh.html

find . -mtime -7 -type f
来源：http://hz.guannengcc.top/gtguaccjia.html

[R45] 批量删除
来源：http://hz.vqdsnc.cn/gtbjkcgjmj.html

find . -name "*.tmp" -delete
来源：http://hz.fzhhl.top/gtpunzhent.html

[R46] 递归替换文件内容
来源：http://hz.wangdashe.top/gtavilgnhw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.c1oappe.top/gtkmirhvug.html

[R47] sed 单行替换
来源：http://hz.yj20258888.top/gtvdqffndz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.9152youxi.cn/gtvrihcleo.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtsjymhebv.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtcnvjidgm.html

[R49] awk 带条件
来源：http://hz.sysykeji.top/gtrwlmhrzc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xuanzx.com/gtuwubczxc.html

[R50] awk 求和
来源：http://hz.pengpengdd.cyou/gtwygfwhwf.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.havefunace.top/gtfwnkcsoc.html

[R51] 排序去重取前几
来源：http://hz.zhijiandao.cn/gtrbtmvdve.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.svipenyu.cn/gttotzchmw.html

[R52] 统计行数
来源：http://hz.hfpthk.cn/gtpeumegqk.html

wc -l a.txt
来源：http://hz.ydzc1.top/gtyjfgrsnh.html

[R53] 查看文件头与实时尾
来源：http://hz.pengpengdd.cyou/gtpsypvgtb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtetvepiec.html

[R54] 比较两个文件
来源：http://hz.ppjwa.cn/gtviskfdxx.html

diff a.txt b.txt
来源：http://hz.hnxiangtu.top/gtcwfdhmqz.html

[R55] 压缩与解压
来源：http://hz.9152youxi.cn/gtndwyqsjy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.yueranfly.top/gtcpsmyapt.html

[R56] 远程拷贝
来源：http://hz.jianghu66.top/gteuctqioc.html

scp file user@host:/path/
来源：http://hz.shuidangran.top/gtlveomnus.html

[R57] 远程执行命令
来源：http://hz.gotoacloud.top/gtfsjgnhuk.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gtkzmnyvzu.html

[R58] 下载文件
来源：http://hz.wangshuangyany.cn/gtoarslrqk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.chenlongwang.top/gtdhhfvhfl.html

[R59] 发 POST JSON
来源：http://hz.shanyushiyangkeji.top/gtegklfyig.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dianchejie.cn/gtnbkhcqjp.html

[R60] 只看 HTTP 状态码
来源：http://hz.meibo888.top/gtysrjqfcm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgfzy.top/gthfardxce.html

[R61] 磁盘占用
来源：http://hz.zdqjudy.top/gtfpbmqwgf.html

df -h;  du -sh *
来源：http://hz.nanxinkj.top/gtzriqtqkq.html

[R62] 找最占空间的文件
来源：http://hz.birdmap.top/gtddhkfvjk.html

du -ah . | sort -rh | head -10
来源：http://hz.iojbl.cn/gtmcxmtvef.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtbypunebi.html

free -h;  ps aux | grep nginx
来源：http://hz.jianghu66.top/gtosudeobu.html

[R64] 结束进程
来源：http://hz.ivvv.top/gtihzrqywv.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtqekulwzo.html

[R65] 查看端口占用
来源：http://hz.shangyingyoupin.top/gtiaolsljc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigfzy.top/gtzfklufor.html

[R66] 定时任务
来源：http://hz.nanxuanxn.top/gtavwfcuuj.html

crontab -e;  crontab -l
来源：http://hz.c1oappe.top/gtqmmsckxf.html

[R67] 生成随机十六进制串
来源：http://hz.jinqigufen.top/gtnquucyan.html

openssl rand -hex 16
来源：http://hz.cucudq.cn/gtclmzylgy.html

[R68] 计算文件校验值
来源：http://hz.snrcjt.cn/gtyhuaiewx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gtbaovlexk.html

[R69] 生成随机密码
来源：http://hz.chenzaomai.com/gtlbyffitx.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtjerkvlhe.html

[R70] 时间戳与互转
来源：http://hz.meibo888.top/gtlvcmsvxl.html

date +%s;  date -d @1700000000
来源：http://hz.jyoumei.cn/gtgqhsayts.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gtogxiykpu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtmbshuegw.html

[R72] 等待端口就绪
来源：http://hz.smart0.xyz/gtogsbiflr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtsgfhpmpn.html

[R73] 分割大日志
来源：http://hz.zycfv.cn/gtzpjqcpcw.html

split -l 1000 big.log part_
来源：http://hz.hywenlv.cn/gtomrzkmec.html

[R74] 批量重命名
来源：http://hz.shanyushiyangkeji.top/gtyaprkebq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.vqdsnc.cn/gttgftgoja.html

[R75] 导出环境变量
来源：http://hz.guowangkeji.top/gtzguiaxxv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtrwdvekcj.html

[R76] 使用临时文件
来源：http://hz.daxiang520.top/gtuaxlmdpz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtufnyrojt.html

[R77] 读取用户输入
来源：http://hz.quarkkingdee.top/gtjgupuftm.html

read -rp "请输入: " ans
来源：http://hz.pengpengdd.cyou/gtorpawqtg.html

[R78] 交互式菜单
来源：http://hz.yangfankeji.com/gtnpuwgekx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj202588.top/gtrcoxeils.html

[R79] 解析命令行选项
来源：http://hz.cdnleiting.top/gtqrccklhj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtybvnglhb.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangkeji.top/gtmjvavllf.html

time ./run.sh
来源：http://hz.snrcjt.cn/gtatqulzrv.html

================================================================================
来源：http://hz.zycfv.cn/gtheuzfqip.html

S. C / C++ 专题
来源：http://hz.ybcxt.top/gtepntfhzn.html

================================================================================
来源：http://hz.yvedp.cn/gtbyikfdlr.html

[S01] C：Hello World
来源：http://hz.xziqi.cn/gtcnhzlwaq.html

#include <stdio.h>
来源：http://hz.gzhubu.top/gtbyehfsrc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gtypshnpsq.html

[S02] C：变量与格式化输出
来源：http://hz.gzhubu.top/gtmbfvsptl.html

int a = 10; printf("%d\n", a);
来源：http://hz.xuanzx.com/gtrdhbvehp.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtkhsddloe.html

int x; scanf("%d", &x);
来源：http://hz.hongshengwenyu.top/gtfvatenju.html

[S04] C：字符串复制
来源：http://hz.nanxuanxn.top/gtszsbeiwk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.guowangkeji.top/gtyjkafiyp.html

[S05] C：字符串长度
来源：http://hz.shuidangran.top/gtkxlwqjby.html

strlen(s)
来源：http://hz.jlsjyb.cn/gtmhmygxsa.html

[S06] C：字符串比较
来源：http://hz.hfpthk.cn/gtgergwwkp.html

strcmp(a, b) == 0
来源：http://hz.aibaodan.cn/gtdkldyvxq.html

[S07] C：数组遍历求和
来源：http://hz.pengpengdd.cyou/gtmmjfianz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.redwolf501.top/gtttmlttgi.html

[S08] C：动态内存分配与释放
来源：http://hz.jinghuilouyu.cn/gtmtwraknw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fengsongda.top/gtwjunrknq.html

[S09] C：结构体定义与初始化
来源：http://hz.cashguo.top/gtarcagcsf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.quarkkingdee.top/gtksginvui.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtklvxpspk.html

int *p = &a;  *p = 5;
来源：http://hz.xuanzx.com/gtcwrapsvq.html

[S11] C：逐行读文件
来源：http://hz.tian-w.cn/gtqntekgrn.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.aizwys.cn/gtkglbaimb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pengpengdd.cyou/gtygabtehw.html

fclose(f);
来源：http://hz.zycfv.cn/gtaspndslx.html

[S12] C：写文件
来源：http://hz.fengsongda.top/gtbcvnrmrz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hywenlv.cn/gtsnekbnoy.html

[S13] C：宏定义
来源：http://hz.hnqzz.top/gtrmfvnuqd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.ydjk.org.cn/gtsarcgcyk.html

[S14] C：枚举
来源：http://hz.jinghuilouyu.cn/gtjyiwvsws.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ivvv.top/gtmrcvedin.html

[S15] C：类型转换
来源：http://hz.kuanghao11.cn/gtxlubiylu.html

(double) a / b
来源：http://hz.jyoumei.cn/gtkhynkvmx.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtnhhguybu.html

x |= (1 << 3);
来源：http://hz.tanke756.top/gtbvladnur.html

[S17] C：安全拼接字符串
来源：http://hz.ybcxt.top/gtgoatvzxm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.haohaochexian.top/gtzhrrjzvu.html

[S18] C：命令行参数
来源：http://hz.sxryk.cn/gtlprhfhem.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtsiomabgs.html

[S19] C：快速排序
来源：http://hz.vqdsnc.cn/gtpamzxjgo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtmgaobgzq.html

[S20] C：二分查找
来源：http://hz.yj20258888.top/gtbxwkmagw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.pycfn.com/gtigrzihvf.html

[S21] C：字符类别判断
来源：http://hz.jinqigufen.top/gtinuqrzam.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gtlphqwyah.html

[S22] C：字符串转数字
来源：http://hz.dianchejie.cn/gtdnqfxchn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.316326.xyz/gtvaojewzb.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtevraslyk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgufenzy.top/gtcxbfgjsv.html

[S24] C：获取本地时间
来源：http://hz.cucudq.cn/gtdcvjxngh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuxming.cn/gtubjodgmt.html

[S25] C：内存拷贝
来源：http://hz.chenjidiqi.icu/gtckfbozih.html

memcpy(dst, src, n);
来源：http://hz.daria6918.cn/gtblhwodxd.html

[S26] C：内存清零
来源：http://hz.yonumen.top/gtwjijxwsg.html

memset(a, 0, sizeof a);
来源：http://hz.andypj.xyz/gtbdavswzd.html

[S27] C：定义常量
来源：http://hz.zhengqikj.top/gtqjvqfgxz.html

const double PI = 3.14159;
来源：http://hz.fengsongda.top/gtkibvsvgy.html

[S28] C：静态变量
来源：http://hz.yueranfly.top/gtudcpcmji.html

static int counter = 0;
来源：http://hz.jqgufenzy.top/gtbhlxhcjd.html

[S29] C：变参函数
来源：http://hz.zycfv.cn/gtvvpwhpwb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtivdeblsp.html

[S30] C：头文件保护
来源：http://hz.vqdsnc.cn/gtqbcsodpr.html

#ifndef X_H
来源：http://hz.wangdashe.top/gtcnhtyret.html

#define X_H
来源：http://hz.aizwys.cn/gtqygwkeco.html

#endif
来源：http://hz.iojbl.cn/gtuwpaajdk.html

[S31] C++：Hello World
来源：http://hz.nanxinkj.top/gtpcbuhiwp.html

#include <iostream>
来源：http://hz.cucudq.cn/gtlcniwwij.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenzaomai.com/gtgpowudzr.html

[S32] C++：字符串
来源：http://hz.hnxiangtu.top/gtnnkxnzjg.html

std::string s = "hi";  s += "!";
来源：http://hz.shanyushiyangkeji.top/gtutamctxj.html

[S33] C++：vector 增删
来源：http://hz.haohaochexian.top/gtgsunypjd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sxryk.cn/gttlqswezv.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtpdiwziia.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.tanke756.top/gtcmytphff.html

[S35] C++：map
来源：http://hz.zhoulong.xyz/gtjahnnved.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cdnleiting.top/gtfytzrdpp.html

[S36] C++：unordered_map
来源：http://hz.xingfuxueyuan.xyz/gtaetwkugy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtihvugbhz.html

[S37] C++：set
来源：http://hz.xuetiantiany.cn/gtpdvqsxsq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.andypj.xyz/gtpmvrladb.html

[S38] C++：排序
来源：http://hz.52xcode.cn/gtsuwiwfoe.html

std::sort(v.begin(), v.end());
来源：http://hz.tian-w.cn/gtaidbpaax.html

[S39] C++：自定义比较器排序
来源：http://hz.jinqigfzy.top/gtgoidknom.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258.top/gtpzbxkygz.html

[S40] C++：查找元素
来源：http://hz.meibo888.top/gticpizgnn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtmjwhbkpw.html

[S41] C++：类与构造函数
来源：http://hz.zdqjudy.top/gtxclqmjfu.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.andypj.xyz/gtrucxwctb.html

[S42] C++：继承与虚函数
来源：http://hz.pycfn.com/gtxrkilpjy.html

class B : public Base { public: void f() override {} };
来源：http://hz.zycfv.cn/gttkckasgg.html

[S43] C++：智能指针
来源：http://hz.jinyuanbaomall.cn/gtmfemljqj.html

auto p = std::make_unique<int>(5);
来源：http://hz.dianchejie.cn/gttmxjrpnp.html

[S44] C++：引用传参
来源：http://hz.xziqi.cn/gtpsrajeqe.html

void inc(int &x) { ++x; }
来源：http://hz.shanyushiyangkeji.top/gtiwzhcvna.html

[S45] C++：lambda
来源：http://hz.zhengqikj.top/gtmblrqylv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.meibo888.top/gtqntvkxxd.html

[S46] C++：函数模板
来源：http://hz.pycfn.com/gtmezowksk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.yuxming.cn/gtjokjkfkn.html

[S47] C++：结构化绑定遍历
来源：http://hz.zdqjudy.top/gthyqsuviq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinyuanbaomall.cn/gtsjlkflcd.html

[S48] C++：逐行读文件
来源：http://hz.zycfv.cn/gtoniiulof.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hongshengwenyu.top/gttsasainn.html

while (std::getline(in, line)) { }
来源：http://hz.zdqjudy.top/gtzoapdawp.html

[S49] C++：写文件
来源：http://hz.ivvv.top/gtqhgsrzui.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tianlin.xyz/gtcoxubcjt.html

[S50] C++：格式化数字
来源：http://hz.wangdashe.top/gtirjmlqxb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhiwuduotai.top/gtqqnogutr.html

[S51] C++：显式类型转换
来源：http://hz.yanxiufei.cn/gtzxupnetj.html

static_cast<double>(a) / b
来源：http://hz.kuanghao11.cn/gtnxoeirqj.html

[S52] C++：const 与 noexcept
来源：http://hz.52xcode.cn/gtshqbsmhw.html

int size() const noexcept { return n_; }
来源：http://hz.shuidangran.top/gtnctzuxjg.html

[S53] C++：移动语义
来源：http://hz.andypj.xyz/gtdrbchkfm.html

std::vector<int> w = std::move(v);
来源：http://hz.jinyuanbaomall.cn/gtybgryztp.html

[S54] C++：异常处理
来源：http://hz.daria6918.cn/gtagklcaxz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.sufxvd.cn/gtintcopkp.html

[S55] C++：结构化绑定
来源：http://hz.nanxuanxn.top/gtdtucodzm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.feifeiyinyue.top/gtoirlxvyu.html

[S56] C++：optional
来源：http://hz.dianchejie.cn/gtsneobmrz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jqgfzy.top/gtfzquxqjv.html

[S57] C++：编译期常量
来源：http://hz.yuxming.cn/gtinwabafh.html

constexpr int N = 10;
来源：http://hz.ehwqpu.com/gtvionzzay.html

[S58] C++：命名空间
来源：http://hz.jinyuanbaomall.cn/gtfdalcjon.html

namespace ns { int f() { return 1; } }
来源：http://hz.daria6918.cn/gtenppfemy.html

[S59] C++：静态断言
来源：http://hz.aibaodan.cn/gthdeeomgt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.pycfn.com/gtudnppegu.html

[S60] C++：遍历并删除元素
来源：http://hz.shzxlz.cn/gtcgsewose.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sufxvd.cn/gtpmorgsgp.html

================================================================================
来源：http://hz.ydzc1.top/gtnxsrzpxc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.kuanghao11.cn/gtvhrisnxu.html

================================================================================
来源：http://hz.yj202588.top/gtyxglusyk.html

[T01] Kotlin：Hello World
来源：http://hz.guannengcc.top/gtltgzjrfp.html

println("Hello")
来源：http://hz.zhoulong.xyz/gtaocrblck.html

[T02] Kotlin：变量
来源：http://hz.meibo888.top/gtulxzfswz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.nwbrower.top/gtvqudyatp.html

[T03] Kotlin：字符串模板
来源：http://hz.redwolf501.top/gtglqahymk.html

"值: $b"
来源：http://hz.xinyue.icu/gtupizeuay.html

[T04] Kotlin：空安全
来源：http://hz.wangdashe.top/gtydjhnmen.html

val n: String? = null;  n?.length
来源：http://hz.zhengqikj.top/gtxovdxfkl.html

[T05] Kotlin：when 表达式
来源：http://hz.aibaodan.cn/gtfrtkfwnf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.haohaochexian.top/gtivmlqkmd.html

[T06] Kotlin：集合映射
来源：http://hz.yj202588.top/gtnqncovmj.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.pycfn.com/gtpeernzal.html

[T07] Kotlin：集合过滤
来源：http://hz.sxryk.cn/gtpxpladef.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.nwbrower.top/gtufnsbrjd.html

[T08] Kotlin：数据类
来源：http://hz.yuxming.cn/gtogbvfakd.html

data class User(val name: String, val age: Int)
来源：http://hz.aizwys.cn/gtabvsrbem.html

[T09] Kotlin：扩展函数
来源：http://hz.zdqjudy.top/gtezuqklxk.html

fun String.exclaim() = this + "!"
来源：http://hz.ivvv.top/gtebzikdjk.html

[T10] Kotlin：默认参数
来源：http://hz.hnqzz.top/gtfitushzb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hammf.cn/gttuguvbpu.html

[T11] Kotlin：协程
来源：http://hz.iojbl.cn/gtymvjlfmm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258.top/gthbggytvx.html

[T12] Kotlin：解构声明
来源：http://hz.tian-w.cn/gtwcdcjvyz.html

val (a, b) = Pair(1, 2)
来源：http://hz.chenlongwang.top/gtdbmchfwl.html

[T13] Kotlin：只读 Map
来源：http://hz.tianlin.xyz/gtzgnruqwe.html

val m = mapOf("a" to 1)
来源：http://hz.shzxlz.cn/gtmtzxjpbx.html

[T14] Kotlin：循环
来源：http://hz.ehwqpu.com/gtzqqvqkkk.html

for (i in 1..10) println(i)
来源：http://hz.yueranfly.top/gthglzwpwa.html

[T15] Kotlin：接口
来源：http://hz.shzxlz.cn/gtxfpcuigb.html

interface Shape { fun area(): Double }
来源：http://hz.kuanghao11.cn/gtzrjncweu.html

[T16] Swift：Hello World
来源：http://hz.zhiwuduotai.top/gtjixtsfxe.html

print("Hello")
来源：http://hz.wangdashe.top/gtdcdpwian.html

[T17] Swift：变量与常量
来源：http://hz.bjfxy.top/gtfvnrawtq.html

var a = 1;  let b = 2
来源：http://hz.hnxiangtu.top/gtpzzcsbni.html

[T18] Swift：字符串插值
来源：http://hz.fengsongda.top/gtinmjfinv.html

"值: \(b)"
来源：http://hz.havefunace.top/gtalonlwuy.html

[T19] Swift：可选绑定
来源：http://hz.shzxlz.cn/gtkdljhdfc.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gtnxcvvjbv.html

[T20] Swift：数组操作
来源：http://hz.jinghuilouyu.cn/gtiyfwtklb.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhaomingkeji.xyz/gthvzmqyvt.html

[T21] Swift：遍历
来源：http://hz.daria6918.cn/gtceycfcoj.html

for x in a { print(x) }
来源：http://hz.wangdashe.top/gtilmuvnwo.html

[T22] Swift：字典
来源：http://hz.chenjidiqi.icu/gtirsqukrk.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.svipenyu.cn/gtrsgztkdq.html

[T23] Swift：函数
来源：http://hz.xinyue.icu/gtteggnkgy.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.daria6918.cn/gtxripdgdx.html

[T24] Swift：闭包
来源：http://hz.pengpengdd.cyou/gtkjzznfgg.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.ywan-chungtsiang.top/gthtdnnxrh.html


<!-- 参考信息 -->