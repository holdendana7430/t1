代发 wailian999

echo "${#s}"
来源：http://hz.redwolf501.top/gtllrjcpgo.html

[R22] 截取子串
来源：http://hz.hammf.cn/gtpbqqvaak.html

echo "${s:0:5}"
来源：http://hz.yonumen.top/gthvgeqvdn.html

[R23] 字符串替换
来源：http://hz.tian-w.cn/gtqmjfimjn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.dianchejie.cn/gtovsrbaxr.html

[R24] 大小写转换
来源：http://hz.tianlin.xyz/gtxwtvqxme.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.quarkkingdee.top/gtjetyepyp.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtjlqjwxzt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aibaodan.cn/gtlqzewmja.html

[R26] 命令替换
来源：http://hz.yvedp.cn/gtrinbfkqf.html

now=$(date +%F); echo "$now"
来源：http://hz.shanyushiyangkeji.top/gtfkqurjig.html

[R27] 算术展开
来源：http://hz.zhengqikj.top/gtyuybzyzw.html

echo $((1 + 2 * 3))
来源：http://hz.tanke756.top/gtscthcnfp.html

[R28] 浮点运算
来源：http://hz.wangshuangyany.cn/gthennvvfq.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gttbkqkqlm.html

[R29] 定义函数
来源：http://hz.hysaishi.cn/gtpqwbpzdv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtcgpfyisy.html

[R30] 函数返回状态码
来源：http://hz.zycfv.cn/gtmrvmwyxz.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhijiandao.cn/gtjvjblihm.html

[R31] 局部变量
来源：http://hz.zhixingplan.top/gtbilzpzri.html

f() { local x=1; echo "$x"; }
来源：http://hz.jyoumei.cn/gtfavyikrn.html

[R32] 参数个数校验
来源：http://hz.aizwys.cn/gteybptafj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.wangshuangyany.cn/gtpkfjdhpl.html

[R33] 捕获错误并提示行号
来源：http://hz.ywan-chungtsiang.top/gtimdbnlxi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhengqikj.top/gtotdktpzi.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtvpimmvyf.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ywan-chungtsiang.top/gtflmjuiox.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtpzvqtebg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.cheryme.top/gtqloyssqz.html

[R36] 并发执行多个任务
来源：http://hz.yj20258.top/gtzgwsmwwk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shangyingyoupin.top/gtkamgoyjj.html

[R37] 把输出赋给变量
来源：http://hz.0kj1m.cn/gtgldibtdt.html

files=$(ls -1)
来源：http://hz.sxryk.cn/gtfvitgdwl.html

[R38] 管道串联
来源：http://hz.quarkkingdee.top/gtibnaxmgb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhongyouzk.top/gtudzbvnpy.html

[R39] 重定向标准输出与错误
来源：http://hz.guannengcc.top/gtiqpoepqy.html

cmd > out.log 2>&1
来源：http://hz.fengsongda.top/gtgpnobnui.html

[R40] 追加写日志
来源：http://hz.xuetiantiany.cn/gtgcnosjzq.html

echo "log" >> out.log
来源：http://hz.zhaomingkeji.xyz/gtotrcdgep.html

[R41] 丢弃输出
来源：http://hz.yj202588.top/gtavyoeioq.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtuklmliam.html

[R42] 输入重定向
来源：http://hz.meibo888.top/gtlkdfqgjx.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtrgwxigur.html

[R43] 按名字查找文件
来源：http://hz.quarkkingdee.top/gtukjjbgoj.html

find . -name "*.log" -type f
来源：http://hz.hysaishi.cn/gtwjvjkaal.html

[R44] 按修改时间查找
来源：http://hz.yj202588.top/gtskhcautu.html

find . -mtime -7 -type f
来源：http://hz.svipenyu.cn/gtmtbfiiuh.html

[R45] 批量删除
来源：http://hz.pycfn.com/gturbqmkqf.html

find . -name "*.tmp" -delete
来源：http://hz.iojbl.cn/gthucoxmfv.html

[R46] 递归替换文件内容
来源：http://hz.wangdashe.top/gtygiqufbu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258888.top/gtaookmism.html

[R47] sed 单行替换
来源：http://hz.hnxiangtu.top/gtsweskfpx.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.wangdashe.top/gtumipebhh.html

[R48] awk 取指定列
来源：http://hz.cqqwz.cn/gttxkdjekn.html

awk '{print $1, $3}' a.txt
来源：http://hz.0kj1m.cn/gtbscvtwtm.html

[R49] awk 带条件
来源：http://hz.daria6918.cn/gtrrwiodhk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.wangshuangyany.cn/gtfjzhwvic.html

[R50] awk 求和
来源：http://hz.chenlongwang.top/gtexinmvkz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hywenlv.cn/gtiblhrqsg.html

[R51] 排序去重取前几
来源：http://hz.xuetiantiany.cn/gtvvexjjhh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yongpay.top/gtwemfgsfy.html

[R52] 统计行数
来源：http://hz.xuanzx.com/gtculvxqee.html

wc -l a.txt
来源：http://hz.quarkkingdee.top/gtzcboftzx.html

[R53] 查看文件头与实时尾
来源：http://hz.dashuyun.cn/gtmtjudznz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.yangfankeji.com/gtzrumxdyg.html

[R54] 比较两个文件
来源：http://hz.chenlongwang.top/gtyllssmox.html

diff a.txt b.txt
来源：http://hz.hywenlv.cn/gttmypgepb.html

[R55] 压缩与解压
来源：http://hz.jinyuanbaomall.cn/gthaxhvefg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gogol.net.cn/gtcimmobnj.html

[R56] 远程拷贝
来源：http://hz.cashguo.top/gtzkjzouvq.html

scp file user@host:/path/
来源：http://hz.shanyushiyangtech.top/gtcaqegoee.html

[R57] 远程执行命令
来源：http://hz.316326.xyz/gtthsmhbci.html

ssh user@host 'uptime'
来源：http://hz.yongpay.top/gttjojewwt.html

[R58] 下载文件
来源：http://hz.tanke756.top/gtmcfjjvsj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yj202588.top/gtxdlptykw.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gtgtimsaca.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hnqzz.top/gtnwcsjhus.html

[R60] 只看 HTTP 状态码
来源：http://hz.havefunace.top/gtprnlaqbi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.ybcxt.top/gtojwebpgm.html

[R61] 磁盘占用
来源：http://hz.guannengcc.top/gtjziwxxig.html

df -h;  du -sh *
来源：http://hz.ybcxt.top/gtmlhqoxqw.html

[R62] 找最占空间的文件
来源：http://hz.jqgufenzy.top/gtxewtxkib.html

du -ah . | sort -rh | head -10
来源：http://hz.ydjk.org.cn/gtubdjprdl.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gtdfdewuxw.html

free -h;  ps aux | grep nginx
来源：http://hz.daria6918.cn/gtahmaltuq.html

[R64] 结束进程
来源：http://hz.tian-w.cn/gtewksxigl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.redwolf501.top/gtvvplqpgm.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtcanjksax.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aizwys.cn/gtrfaadfjn.html

[R66] 定时任务
来源：http://hz.tian-w.cn/gtvkzaxqln.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtkmlsqwcj.html

[R67] 生成随机十六进制串
来源：http://hz.9152youxi.cn/gtrkjwovde.html

openssl rand -hex 16
来源：http://hz.hongshengwenyu.top/gtmesihrra.html

[R68] 计算文件校验值
来源：http://hz.ywan-chungtsiang.top/gtlwkgklfv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jyoumei.cn/gtcrcyguiq.html

[R69] 生成随机密码
来源：http://hz.hfpthk.cn/gtuaiyrpfy.html

head -c 16 /dev/urandom | base64
来源：http://hz.tian-w.cn/gtsxuzoddu.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtjvixtdjl.html

date +%s;  date -d @1700000000
来源：http://hz.havefunace.top/gtjhgglwtm.html

[R71] 日期格式化
来源：http://hz.yuxming.cn/gtaawbnhdj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.havefunace.top/gtvzvjkamy.html

[R72] 等待端口就绪
来源：http://hz.yj20258888.top/gtgpfdglcr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.havefunace.top/gttcbvivbh.html

[R73] 分割大日志
来源：http://hz.zhaomingkeji.xyz/gtwhddseda.html

split -l 1000 big.log part_
来源：http://hz.sufxvd.cn/gtgpjydmic.html

[R74] 批量重命名
来源：http://hz.ydzc1.top/gtzedfbwtv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinghuilouyu.cn/gtgpfqxavj.html

[R75] 导出环境变量
来源：http://hz.tian-w.cn/gtarbqtfhv.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yangfankeji.com/gtifhwnbbp.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtmikoomqp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtcrzjpkiy.html

[R77] 读取用户输入
来源：http://hz.haohaochexian.top/gtudfnxbhw.html

read -rp "请输入: " ans
来源：http://hz.quarkkingdee.top/gtcxddhyle.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtwekpgguu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258.top/gthbwulnfg.html

[R79] 解析命令行选项
来源：http://hz.dashuyun.cn/gtpbsdzkro.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.zycfv.cn/gtynuamreo.html

[R80] 查看脚本执行耗时
来源：http://hz.zhiwuduotai.top/gtphgioufc.html

time ./run.sh
来源：http://hz.ybcxt.top/gtuvffmwnx.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtupryfaok.html

S. C / C++ 专题
来源：http://hz.cucudq.cn/gtwihwoiep.html

================================================================================
来源：http://hz.aizwys.cn/gthsgzmsjz.html

[S01] C：Hello World
来源：http://hz.yanxiufei.cn/gtmxznbrmw.html

#include <stdio.h>
来源：http://hz.birdmap.top/gtxcsbemuv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhijiandao.cn/gtvndxdcem.html

[S02] C：变量与格式化输出
来源：http://hz.hnqzz.top/gtheawuuba.html

int a = 10; printf("%d\n", a);
来源：http://hz.sxryk.cn/gtrozwmfnd.html

[S03] C：读入整数
来源：http://hz.pengpengdd.cyou/gtmvoegnxi.html

int x; scanf("%d", &x);
来源：http://hz.316326.xyz/gtjmmpowhh.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtbozbpcmd.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtwzurjbgk.html

[S05] C：字符串长度
来源：http://hz.meibo888.top/gtgjuqwwcn.html

strlen(s)
来源：http://hz.andypj.xyz/gtnpsqfknh.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtacngpnmh.html

strcmp(a, b) == 0
来源：http://hz.guannengcc.top/gtwlrkhzwu.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtusaaoezc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj202588.top/gtorkmcxgv.html

[S08] C：动态内存分配与释放
来源：http://hz.shanyushiyangkeji.top/gtwdsddbmg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zycfv.cn/gtoucddaup.html

[S09] C：结构体定义与初始化
来源：http://hz.ppjwa.cn/gtqzytdolg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhongyouzk.top/gtoiilmkei.html

[S10] C：指针与解引用
来源：http://hz.shzxlz.cn/gtbrxzxdzu.html

int *p = &a;  *p = 5;
来源：http://hz.meibo888.top/gtiutbtpcw.html

[S11] C：逐行读文件
来源：http://hz.andypj.xyz/gtmuetmscu.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.zycfv.cn/gtrebrhvqp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.pengpengdd.cyou/gtfsffqnmc.html

fclose(f);
来源：http://hz.xinyue.icu/gtwytoivzu.html

[S12] C：写文件
来源：http://hz.tianlin.xyz/gtjhjuyzja.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yonumen.top/gttkcmhavf.html

[S13] C：宏定义
来源：http://hz.ydzc1.top/gtqqltqeiw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hysaishi.cn/gtcsnfpezh.html

[S14] C：枚举
来源：http://hz.jqgufenzy.top/gtgtomgfbh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hywenlv.cn/gtwoatbphj.html

[S15] C：类型转换
来源：http://hz.jiagoushi.top/gtdnnjqerq.html

(double) a / b
来源：http://hz.xingfuxueyuan.xyz/gtpmaemvyl.html

[S16] C：位操作置位
来源：http://hz.nanxuanxn.top/gtwyjjupeh.html

x |= (1 << 3);
来源：http://hz.c1oappe.top/gttwvnbvun.html

[S17] C：安全拼接字符串
来源：http://hz.aibaodan.cn/gtdsfwxddm.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zdqjudy.top/gtdmesspka.html

[S18] C：命令行参数
来源：http://hz.yvedp.cn/gtssphleug.html

int main(int argc, char **argv)
来源：http://hz.cheryme.top/gtlfviaqmz.html

[S19] C：快速排序
来源：http://hz.snrcjt.cn/gtinuklilx.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.feifeiyinyue.top/gtczoutljb.html

[S20] C：二分查找
来源：http://hz.sysykeji.top/gtyeurdjup.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.chenjidiqi.icu/gtbyszegmz.html

[S21] C：字符类别判断
来源：http://hz.hammf.cn/gtakcgqfbm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yongpay.top/gtylbpxypv.html

[S22] C：字符串转数字
来源：http://hz.cucudq.cn/gtdadlqbkv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.316326.xyz/gtnmlvyhxv.html

[S23] C：随机数
来源：http://hz.jyoumei.cn/gtaufyzvwx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgfzy.top/gtjrhzygri.html

[S24] C：获取本地时间
来源：http://hz.hnqzz.top/gtjxdkbdrj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yj20258888.top/gtzppqpdmh.html

[S25] C：内存拷贝
来源：http://hz.xuetiantiany.cn/gtrjgexsly.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtcbajyvzo.html

[S26] C：内存清零
来源：http://hz.daxiang520.top/gtpxkzbfkk.html

memset(a, 0, sizeof a);
来源：http://hz.dianchejie.cn/gtelcqtfbm.html

[S27] C：定义常量
来源：http://hz.haohaochexian.top/gtmydksevj.html

const double PI = 3.14159;
来源：http://hz.haohaochexian.top/gtpesvagoc.html

[S28] C：静态变量
来源：http://hz.wangdashe.top/gtrlgudwyx.html

static int counter = 0;
来源：http://hz.cashguo.top/gtusfumvcl.html

[S29] C：变参函数
来源：http://hz.snrcjt.cn/gtfkqimsms.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhongyouzk.top/gtaiyghmsk.html

[S30] C：头文件保护
来源：http://hz.gaohongyu789.top/gtzjfshxne.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtdpzyoyvk.html

#define X_H
来源：http://hz.52xcode.cn/gticefmatb.html

#endif
来源：http://hz.ppjwa.cn/gtdrygkmkr.html

[S31] C++：Hello World
来源：http://hz.guowangkeji.top/gtpwgrhydr.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtcdflctnx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.mhx1999.top/gthxlfhkoo.html

[S32] C++：字符串
来源：http://hz.pengpengdd.cyou/gtgnxjdrwh.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtiuyxrmni.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtdjrzqnja.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.52xcode.cn/gtqirrhdiy.html

[S34] C++：遍历 vector
来源：http://hz.gaohongyu789.top/gtsguvgrxr.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.cucudq.cn/gtjtymqnhl.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtzikwyenb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.0kj1m.cn/gtiqkibmin.html

[S36] C++：unordered_map
来源：http://hz.ehwqpu.com/gttqzmzabq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xinyue.icu/gtuvnuieot.html

[S37] C++：set
来源：http://hz.tianlin.xyz/gtzddmoigu.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.daxiang520.top/gthtiflyly.html

[S38] C++：排序
来源：http://hz.chenzaomai.com/gthqgadfku.html

std::sort(v.begin(), v.end());
来源：http://hz.quarkkingdee.top/gtfzrmrdxf.html

[S39] C++：自定义比较器排序
来源：http://hz.zhengqikj.top/gtotdizwlu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.wangdashe.top/gtmaywedwm.html

[S40] C++：查找元素
来源：http://hz.xinyue.icu/gtesudjfau.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jqgfzy.top/gtsmxocrdb.html

[S41] C++：类与构造函数
来源：http://hz.hnqzz.top/gtlskbgvug.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gtwejahojp.html

[S42] C++：继承与虚函数
来源：http://hz.xinyue.icu/gtnwvrgqku.html

class B : public Base { public: void f() override {} };
来源：http://hz.yangfankeji.com/gtpotkbkpi.html

[S43] C++：智能指针
来源：http://hz.shanyushiyangtech.top/gtupnjvjaj.html

auto p = std::make_unique<int>(5);
来源：http://hz.birdmap.top/gtlxpghqze.html

[S44] C++：引用传参
来源：http://hz.iojbl.cn/gtixoxiojc.html

void inc(int &x) { ++x; }
来源：http://hz.sweek.top/gtgfwmrmnn.html

[S45] C++：lambda
来源：http://hz.zycfv.cn/gtswyfvsdk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xylfe.cn/gthgnlgduh.html

[S46] C++：函数模板
来源：http://hz.52xcode.cn/gtfppcckon.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.ydzc1.top/gtkialcimu.html

[S47] C++：结构化绑定遍历
来源：http://hz.meibo888.top/gtjkgateod.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.yangfankeji.com/gtskekuqxn.html

[S48] C++：逐行读文件
来源：http://hz.quarkkingdee.top/gtodjpanfs.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangshuangyany.cn/gtqdhhcred.html

while (std::getline(in, line)) { }
来源：http://hz.hammf.cn/gtughmeqqb.html

[S49] C++：写文件
来源：http://hz.iojbl.cn/gtowbvtdev.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.bjfxy.top/gtgcuxudad.html

[S50] C++：格式化数字
来源：http://hz.ywan-chungtsiang.top/gtvpjggyrq.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.52xcode.cn/gtzxshckpq.html

[S51] C++：显式类型转换
来源：http://hz.cashguo.top/gtowibsjlj.html

static_cast<double>(a) / b
来源：http://hz.shzxlz.cn/gtegmlozjz.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtauunmtof.html

int size() const noexcept { return n_; }
来源：http://hz.hammf.cn/gtryegucxx.html

[S53] C++：移动语义
来源：http://hz.vqdsnc.cn/gtcijwjfnd.html

std::vector<int> w = std::move(v);
来源：http://hz.cdnleiting.top/gtdquvzalk.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtngpknfvd.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.yongpay.top/gtmrmsbbbf.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gtoclhxwsi.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gtwqgirepk.html

[S56] C++：optional
来源：http://hz.tian-w.cn/gtbbpjslkv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yvedp.cn/gtsajlyoso.html

[S57] C++：编译期常量
来源：http://hz.cdnleiting.top/gtihhzbaih.html

constexpr int N = 10;
来源：http://hz.zhijiandao.cn/gtcelykgvo.html

[S58] C++：命名空间
来源：http://hz.guowangkeji.top/gtynkauuqz.html

namespace ns { int f() { return 1; } }
来源：http://hz.meibo888.top/gtvfylsefe.html

[S59] C++：静态断言
来源：http://hz.jlsjyb.cn/gtjhfrmtlv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.daria6918.cn/gtzptbtlui.html

[S60] C++：遍历并删除元素
来源：http://hz.52xcode.cn/gtheckgfxq.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.redwolf501.top/gtuqryexks.html

================================================================================
来源：http://hz.sufxvd.cn/gtnauaoeda.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhixingplan.top/gtgccyunbw.html

================================================================================
来源：http://hz.nwbrower.top/gtiaxorvrv.html

[T01] Kotlin：Hello World
来源：http://hz.jianghu66.top/gtucvtiqpn.html

println("Hello")
来源：http://hz.jinqigufen.top/gtegymasqx.html

[T02] Kotlin：变量
来源：http://hz.zhaomingkeji.xyz/gtkcuxtkdw.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.ivvv.top/gtyxhemtiv.html

[T03] Kotlin：字符串模板
来源：http://hz.pycfn.com/gtnqtmoqft.html

"值: $b"
来源：http://hz.xziqi.cn/gtcbqrkhtf.html

[T04] Kotlin：空安全
来源：http://hz.aibaodan.cn/gtqcruqizg.html

val n: String? = null;  n?.length
来源：http://hz.daxiang520.top/gtubywmiav.html

[T05] Kotlin：when 表达式
来源：http://hz.yvedp.cn/gtaqybojbz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sufxvd.cn/gtbgtmfrom.html

[T06] Kotlin：集合映射
来源：http://hz.xziqi.cn/gtwsfjysyb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cqqwz.cn/gthnrhthcn.html

[T07] Kotlin：集合过滤
来源：http://hz.yongpay.top/gtuebvrdwg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtmzgtfnfj.html

[T08] Kotlin：数据类
来源：http://hz.snrcjt.cn/gtojbdfovo.html

data class User(val name: String, val age: Int)
来源：http://hz.zhoulong.xyz/gtfndgeepy.html

[T09] Kotlin：扩展函数
来源：http://hz.shanyushiyangtech.top/gtcdrezrdf.html

fun String.exclaim() = this + "!"
来源：http://hz.yanxiufei.cn/gtbytmkdaf.html

[T10] Kotlin：默认参数
来源：http://hz.yueranfly.top/gtohtnjiqv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jinqigfzy.top/gtjdmixbfu.html

[T11] Kotlin：协程
来源：http://hz.hnxiangtu.top/gtervzmlee.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenzaomai.com/gtjwonrfkj.html

[T12] Kotlin：解构声明
来源：http://hz.hysaishi.cn/gtiqkfulpr.html

val (a, b) = Pair(1, 2)
来源：http://hz.tanke756.top/gtkcxorvwp.html

[T13] Kotlin：只读 Map
来源：http://hz.zhaomingkeji.xyz/gtvvtqrrrt.html

val m = mapOf("a" to 1)
来源：http://hz.cashguo.top/gtzwvspfed.html

[T14] Kotlin：循环
来源：http://hz.smart0.xyz/gtupbfhmwh.html

for (i in 1..10) println(i)
来源：http://hz.dianchejie.cn/gtmghtzlvf.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtsxjnxxuz.html

interface Shape { fun area(): Double }
来源：http://hz.wangdashe.top/gtnwrqdedc.html

[T16] Swift：Hello World
来源：http://hz.yvedp.cn/gtgmpulfwe.html

print("Hello")
来源：http://hz.daxiang520.top/gtempbbbac.html

[T17] Swift：变量与常量
来源：http://hz.xuetiantiany.cn/gteqqplwxb.html

var a = 1;  let b = 2
来源：http://hz.ivvv.top/gtegrqkcfw.html

[T18] Swift：字符串插值
来源：http://hz.jlsjyb.cn/gtywdijdud.html

"值: \(b)"
来源：http://hz.birdmap.top/gtxrmpcoxy.html

[T19] Swift：可选绑定
来源：http://hz.chenlongwang.top/gtykowyack.html

if let n = opt { print(n) }
来源：http://hz.yanxiufei.cn/gteqaggeou.html

[T20] Swift：数组操作
来源：http://hz.jianghu66.top/gtbbrdsuwk.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.zhijiandao.cn/gtuwydfdmr.html

[T21] Swift：遍历
来源：http://hz.jianghu66.top/gtbvwvmfvm.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtgntivkro.html

[T22] Swift：字典
来源：http://hz.sweek.top/gtideztaan.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.ydjk.org.cn/gtpiszvbjs.html

[T23] Swift：函数
来源：http://hz.0kj1m.cn/gtasffhoat.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.fzhhl.top/gtjtodvrza.html

[T24] Swift：闭包
来源：http://hz.gotoacloud.top/gtpvvfzjzf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.yj20258888.top/gtzgdukvow.html


<!-- 参考信息 -->