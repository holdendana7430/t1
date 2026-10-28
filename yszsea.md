代发 wailian999

echo "${#arr[@]}"
来源：http://hz.ybcxt.top/gtchcqfabp.html

[R20] 关联数组（字典）
来源：http://hz.fengsongda.top/gttkwtdqyf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxuanxn.top/gtblnnfqbx.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtlkaypqqf.html

echo "${#s}"
来源：http://hz.dashuyun.cn/gtlvvcmniv.html

[R22] 截取子串
来源：http://hz.pycfn.com/gtzmxxahhg.html

echo "${s:0:5}"
来源：http://hz.hysaishi.cn/gtjrqaluve.html

[R23] 字符串替换
来源：http://hz.chenzaomai.com/gtrjvqhiyz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hammf.cn/gtwdqgrbiy.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gthrsrtwby.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jyoumei.cn/gthkmcawab.html

[R25] 去后缀 / 去前缀
来源：http://hz.jianghu66.top/gtolpqceol.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.9152youxi.cn/gtvbpebjum.html

[R26] 命令替换
来源：http://hz.cucudq.cn/gtunkoyymi.html

now=$(date +%F); echo "$now"
来源：http://hz.yj202588.top/gtunaelxif.html

[R27] 算术展开
来源：http://hz.bjfxy.top/gtwgaplhhv.html

echo $((1 + 2 * 3))
来源：http://hz.hnqzz.top/gtklgfynkh.html

[R28] 浮点运算
来源：http://hz.cdnleiting.top/gtzgclagzd.html

echo "scale=2; 10/3" | bc
来源：http://hz.ywan-chungtsiang.top/gtpdlvtkvq.html

[R29] 定义函数
来源：http://hz.nanxuanxn.top/gtdedrjqxe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.316326.xyz/gtmhkhsmrk.html

[R30] 函数返回状态码
来源：http://hz.zhengqikj.top/gttngboelo.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnxiangtu.top/gtvcqtnyqb.html

[R31] 局部变量
来源：http://hz.nanxuanxn.top/gtqfefjqje.html

f() { local x=1; echo "$x"; }
来源：http://hz.xylfe.cn/gtszzoztfd.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtnxlwpyrw.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.quarkkingdee.top/gtmteqkzkv.html

[R33] 捕获错误并提示行号
来源：http://hz.jinghuilouyu.cn/gteganoyep.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.cheryme.top/gtfpxgqbzd.html

[R34] 退出时清理
来源：http://hz.tanke756.top/gtbeuohxxt.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangdashe.top/gtomjqsfpi.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtdgaxscdn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shuidangran.top/gtxqxgfkvd.html

[R36] 并发执行多个任务
来源：http://hz.chenlongwang.top/gtzxqvsziy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.gaohongyu789.top/gtxqmcuakf.html

[R37] 把输出赋给变量
来源：http://hz.redwolf501.top/gtdkfpnlqp.html

files=$(ls -1)
来源：http://hz.tian-w.cn/gthjqbrcia.html

[R38] 管道串联
来源：http://hz.sysykeji.top/gtelifvawz.html

cat a.txt | grep -i error | wc -l
来源：http://hz.xinyue.icu/gtuhmbaqqk.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxinkj.top/gthjjgqpcw.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtrhjhomub.html

[R40] 追加写日志
来源：http://hz.fengsongda.top/gtkpytropo.html

echo "log" >> out.log
来源：http://hz.hysaishi.cn/gtzzkzwwxx.html

[R41] 丢弃输出
来源：http://hz.ehwqpu.com/gtvpnmrheh.html

cmd >/dev/null 2>&1
来源：http://hz.ydzc1.top/gtasufiljv.html

[R42] 输入重定向
来源：http://hz.xuetiantiany.cn/gtxranudnf.html

wc -l < a.txt
来源：http://hz.cucudq.cn/gtggdejbnk.html

[R43] 按名字查找文件
来源：http://hz.jqgfzy.top/gttozfoafv.html

find . -name "*.log" -type f
来源：http://hz.sysykeji.top/gtzbxgbpup.html

[R44] 按修改时间查找
来源：http://hz.hfpthk.cn/gtlynxefdh.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gtsijdechp.html

[R45] 批量删除
来源：http://hz.shuidangran.top/gtaxdocpwm.html

find . -name "*.tmp" -delete
来源：http://hz.ydzc1.top/gtgcqxzbjv.html

[R46] 递归替换文件内容
来源：http://hz.zhoulong.xyz/gtlfxhewwr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zhongyouzk.top/gtpadcenny.html

[R47] sed 单行替换
来源：http://hz.aizwys.cn/gtnoyfzrfq.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.tanke756.top/gtrmakvkrp.html

[R48] awk 取指定列
来源：http://hz.cashguo.top/gtuofwilir.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinghuilouyu.cn/gtoxmpymet.html

[R49] awk 带条件
来源：http://hz.tianlin.xyz/gtkseaiekh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.nanxuanxn.top/gtzatsjhfw.html

[R50] awk 求和
来源：http://hz.iojbl.cn/gthrwqzdry.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.snrcjt.cn/gtqirwrhiq.html

[R51] 排序去重取前几
来源：http://hz.pengpengdd.cyou/gttbqzthmr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zycfv.cn/gtqhtgvhjj.html

[R52] 统计行数
来源：http://hz.haohaochexian.top/gtxvjzdlby.html

wc -l a.txt
来源：http://hz.ppjwa.cn/gtklcfpcru.html

[R53] 查看文件头与实时尾
来源：http://hz.jqgufenzy.top/gtumbcyibd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xuetiantiany.cn/gthbldgaxe.html

[R54] 比较两个文件
来源：http://hz.vqdsnc.cn/gtvrhtzdwz.html

diff a.txt b.txt
来源：http://hz.yonumen.top/gtshzfimmx.html

[R55] 压缩与解压
来源：http://hz.ydjk.org.cn/gtjwddbbjs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nwbrower.top/gtpxdwdfnh.html

[R56] 远程拷贝
来源：http://hz.aibaodan.cn/gtzcuammuk.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtkiepeblk.html

[R57] 远程执行命令
来源：http://hz.fengsongda.top/gtplcaqaje.html

ssh user@host 'uptime'
来源：http://hz.wangshuangyany.cn/gtfwnbjmbw.html

[R58] 下载文件
来源：http://hz.cdnleiting.top/gtpyfhfjdj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.havefunace.top/gthqkxdibf.html

[R59] 发 POST JSON
来源：http://hz.tanke756.top/gtnxjqkcrv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shuidangran.top/gtbjnzrwdl.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgufenzy.top/gthkvdezqp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.shanyushiyangtech.top/gtftavqxii.html

[R61] 磁盘占用
来源：http://hz.52xcode.cn/gtbwfgrymn.html

df -h;  du -sh *
来源：http://hz.bjfxy.top/gtafbtfazz.html

[R62] 找最占空间的文件
来源：http://hz.yuanzhike.top/gtvjnjlnau.html

du -ah . | sort -rh | head -10
来源：http://hz.jqgufenzy.top/gtrulheoxn.html

[R63] 内存与进程
来源：http://hz.yonumen.top/gtriahzswn.html

free -h;  ps aux | grep nginx
来源：http://hz.hfpthk.cn/gtlcjibpzs.html

[R64] 结束进程
来源：http://hz.chenzaomai.com/gtthlxhdjm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zhiwuduotai.top/gtimejixfl.html

[R65] 查看端口占用
来源：http://hz.gotoacloud.top/gtdyeivpsx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xingfuxueyuan.xyz/gtzxwwjjtu.html

[R66] 定时任务
来源：http://hz.snrcjt.cn/gtsldrkete.html

crontab -e;  crontab -l
来源：http://hz.hnxiangtu.top/gtgmzdwahj.html

[R67] 生成随机十六进制串
来源：http://hz.xziqi.cn/gtyhvjtnls.html

openssl rand -hex 16
来源：http://hz.hnqzz.top/gthstxxtfi.html

[R68] 计算文件校验值
来源：http://hz.hongshengwenyu.top/gtafgtqbta.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtfjiykncn.html

[R69] 生成随机密码
来源：http://hz.cqqwz.cn/gtseousktf.html

head -c 16 /dev/urandom | base64
来源：http://hz.chenzaomai.com/gtbmlwdcms.html

[R70] 时间戳与互转
来源：http://hz.smart0.xyz/gtnyqryzir.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtdgegdxgq.html

[R71] 日期格式化
来源：http://hz.cashguo.top/gtcrujapul.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydzc1.top/gtbxtypyst.html

[R72] 等待端口就绪
来源：http://hz.hongshengwenyu.top/gtczdjzjwa.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhaomingkeji.xyz/gthdutxgtc.html

[R73] 分割大日志
来源：http://hz.fengsongda.top/gtireyvzud.html

split -l 1000 big.log part_
来源：http://hz.yuxming.cn/gtqbdooqwk.html

[R74] 批量重命名
来源：http://hz.xinyue.icu/gturanffwm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.andypj.xyz/gtstebbocr.html

[R75] 导出环境变量
来源：http://hz.52xcode.cn/gtzihjufnp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtcpyxkocu.html

[R76] 使用临时文件
来源：http://hz.nanxinkj.top/gtzerkrnmy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.guowangkeji.top/gtooszqgcu.html

[R77] 读取用户输入
来源：http://hz.cheryme.top/gtuuzcelqy.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtifftfgmk.html

[R78] 交互式菜单
来源：http://hz.nanxinkj.top/gtssopsiwc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.haohaochexian.top/gtkinuplky.html

[R79] 解析命令行选项
来源：http://hz.yuxming.cn/gtgsuhhnop.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tianlin.xyz/gtlojokhth.html

[R80] 查看脚本执行耗时
来源：http://hz.fengsongda.top/gteunvbtht.html

time ./run.sh
来源：http://hz.dashuyun.cn/gtamtduccm.html

================================================================================
来源：http://hz.aibaodan.cn/gteezizlyl.html

S. C / C++ 专题
来源：http://hz.jqgufenzy.top/gtmonqbhos.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtmxaqvpuk.html

[S01] C：Hello World
来源：http://hz.redwolf501.top/gtivburmzl.html

#include <stdio.h>
来源：http://hz.hnxiangtu.top/gtlambnymg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.snrcjt.cn/gtgklmjkni.html

[S02] C：变量与格式化输出
来源：http://hz.xuetiantiany.cn/gtqkamnlmr.html

int a = 10; printf("%d\n", a);
来源：http://hz.52xcode.cn/gtetqxauui.html

[S03] C：读入整数
来源：http://hz.ehwqpu.com/gtyijoekmo.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtxzmopxzd.html

[S04] C：字符串复制
来源：http://hz.52xcode.cn/gtqkyhjpvi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ydjk.org.cn/gtnnuirssw.html

[S05] C：字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtripbvltc.html

strlen(s)
来源：http://hz.yonumen.top/gtbjpuvvxp.html

[S06] C：字符串比较
来源：http://hz.ydzc1.top/gtzitavwfo.html

strcmp(a, b) == 0
来源：http://hz.hywenlv.cn/gtfypxdfze.html

[S07] C：数组遍历求和
来源：http://hz.zycfv.cn/gtgffynuao.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.jqgufenzy.top/gtjgurccln.html

[S08] C：动态内存分配与释放
来源：http://hz.jiagoushi.top/gtfxbapeia.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.mhx1999.top/gtzjuhdgtw.html

[S09] C：结构体定义与初始化
来源：http://hz.quarkkingdee.top/gtcsckfzgn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.iojbl.cn/gtjaagafmw.html

[S10] C：指针与解引用
来源：http://hz.guowangkeji.top/gtjonhjayx.html

int *p = &a;  *p = 5;
来源：http://hz.havefunace.top/gtgflzhblg.html

[S11] C：逐行读文件
来源：http://hz.ywan-chungtsiang.top/gtugaxsazx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yongpay.top/gtuqtoybcw.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.snrcjt.cn/gtyugdqeyi.html

fclose(f);
来源：http://hz.c1oappe.top/gtwlmjitli.html

[S12] C：写文件
来源：http://hz.xinyue.icu/gtpfsyoqvb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yvedp.cn/gttvxeyzxp.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtevmlqjmk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shanyushiyangtech.top/gtgxnfmteo.html

[S14] C：枚举
来源：http://hz.nwbrower.top/gtnjkmxmmg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.svipenyu.cn/gtdkgvqzvo.html

[S15] C：类型转换
来源：http://hz.yuxming.cn/gtgrbvfkdm.html

(double) a / b
来源：http://hz.ydjk.org.cn/gtnjspdzrp.html

[S16] C：位操作置位
来源：http://hz.haohaochexian.top/gtbwyujdli.html

x |= (1 << 3);
来源：http://hz.cqqwz.cn/gteunrbbos.html

[S17] C：安全拼接字符串
来源：http://hz.cashguo.top/gtivzvdufh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtzazjyxnr.html

[S18] C：命令行参数
来源：http://hz.chenzaomai.com/gtqkynqeoh.html

int main(int argc, char **argv)
来源：http://hz.jinyuanbaomall.cn/gtofppnwpy.html

[S19] C：快速排序
来源：http://hz.jiagoushi.top/gtuegkqoda.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtchlaqkmz.html

[S20] C：二分查找
来源：http://hz.yvedp.cn/gtimzgvdtd.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gtaidjvywk.html

[S21] C：字符类别判断
来源：http://hz.cashguo.top/gtagtmlkts.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zhiwuduotai.top/gtnqbygslq.html

[S22] C：字符串转数字
来源：http://hz.havefunace.top/gtxhnawjid.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhijiandao.cn/gtnpdnotzd.html

[S23] C：随机数
来源：http://hz.chenzaomai.com/gtdgfnvlyl.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xylfe.cn/gtorlkxjzo.html

[S24] C：获取本地时间
来源：http://hz.zhixingplan.top/gtiplmeomx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtrmxjrvld.html

[S25] C：内存拷贝
来源：http://hz.ydzc1.top/gtxzjfritr.html

memcpy(dst, src, n);
来源：http://hz.guannengcc.top/gtonuhshow.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtduwqqgzl.html

memset(a, 0, sizeof a);
来源：http://hz.pycfn.com/gtwjifqlcq.html

[S27] C：定义常量
来源：http://hz.guannengcc.top/gtatuxcyqq.html

const double PI = 3.14159;
来源：http://hz.pengpengdd.cyou/gtuxhkvtet.html

[S28] C：静态变量
来源：http://hz.cucudq.cn/gtpbsyfaoa.html

static int counter = 0;
来源：http://hz.sysykeji.top/gtrxmstcxg.html

[S29] C：变参函数
来源：http://hz.nanxuanxn.top/gtmhbxucyn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cdnleiting.top/gtqaudnxvw.html

[S30] C：头文件保护
来源：http://hz.ydjk.org.cn/gtnplhelpi.html

#ifndef X_H
来源：http://hz.guannengcc.top/gtwsstifbf.html

#define X_H
来源：http://hz.sxryk.cn/gtlvbzfzld.html

#endif
来源：http://hz.kuanghao11.cn/gtiuwdapvo.html

[S31] C++：Hello World
来源：http://hz.havefunace.top/gtygymiolf.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gteccdbktw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.nanxinkj.top/gtyxoukddt.html

[S32] C++：字符串
来源：http://hz.zhiwuduotai.top/gtzyeiypzo.html

std::string s = "hi";  s += "!";
来源：http://hz.chenjidiqi.icu/gtpnfzmijj.html

[S33] C++：vector 增删
来源：http://hz.yanxiufei.cn/gtssfdkwqd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sufxvd.cn/gtwxrvebwt.html

[S34] C++：遍历 vector
来源：http://hz.shzxlz.cn/gtehvkewuz.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ydjk.org.cn/gtlbsuvxso.html

[S35] C++：map
来源：http://hz.hywenlv.cn/gtujdegmao.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtmzbpggjd.html

[S36] C++：unordered_map
来源：http://hz.chenlongwang.top/gtxgjkjlss.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ybcxt.top/gtxmqqydpb.html

[S37] C++：set
来源：http://hz.zhijiandao.cn/gtnihmguay.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.9152youxi.cn/gtwqkhjang.html

[S38] C++：排序
来源：http://hz.yj20258888.top/gtxmqtxpti.html

std::sort(v.begin(), v.end());
来源：http://hz.sweek.top/gtjpfxrxmq.html

[S39] C++：自定义比较器排序
来源：http://hz.gzhubu.top/gtrpepirxc.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.daxiang520.top/gtmrcofbmw.html

[S40] C++：查找元素
来源：http://hz.yvedp.cn/gtrdhvlnvb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dianchejie.cn/gtqqbvrwyk.html

[S41] C++：类与构造函数
来源：http://hz.pengpengdd.cyou/gtrfswzmjk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jinyuanbaomall.cn/gtystolrhz.html

[S42] C++：继承与虚函数
来源：http://hz.sysykeji.top/gtzknxqodh.html

class B : public Base { public: void f() override {} };
来源：http://hz.shanyushiyangtech.top/gtqsoaxfax.html

[S43] C++：智能指针
来源：http://hz.xziqi.cn/gtkvavgexg.html

auto p = std::make_unique<int>(5);
来源：http://hz.yueranfly.top/gtforltsif.html

[S44] C++：引用传参
来源：http://hz.nwbrower.top/gtdlnssexu.html

void inc(int &x) { ++x; }
来源：http://hz.xingfuxueyuan.xyz/gtygthprwb.html

[S45] C++：lambda
来源：http://hz.tian-w.cn/gtkesljabu.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gtggelpuwl.html

[S46] C++：函数模板
来源：http://hz.jqgfzy.top/gtlsffmkxp.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shangyingyoupin.top/gtfyozkbvw.html

[S47] C++：结构化绑定遍历
来源：http://hz.aizwys.cn/gtcxfapsix.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sufxvd.cn/gtoysyuuhe.html

[S48] C++：逐行读文件
来源：http://hz.hongshengwenyu.top/gtzblwdzux.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.dianchejie.cn/gtwdtonroa.html

while (std::getline(in, line)) { }
来源：http://hz.yanxiufei.cn/gtekqjzjhe.html

[S49] C++：写文件
来源：http://hz.daria6918.cn/gthdzvwbbs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.pengpengdd.cyou/gtulsrfrpo.html

[S50] C++：格式化数字
来源：http://hz.andypj.xyz/gtaxosvlgx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.cheryme.top/gtvnhxkgmn.html

[S51] C++：显式类型转换
来源：http://hz.zycfv.cn/gtghqawuvt.html

static_cast<double>(a) / b
来源：http://hz.cheryme.top/gtuwxkhttv.html

[S52] C++：const 与 noexcept
来源：http://hz.ivvv.top/gthtrykpak.html

int size() const noexcept { return n_; }
来源：http://hz.snrcjt.cn/gtrkbxqydt.html

[S53] C++：移动语义
来源：http://hz.gzhubu.top/gtylgixsin.html

std::vector<int> w = std::move(v);
来源：http://hz.ppjwa.cn/gtumlhenqz.html

[S54] C++：异常处理
来源：http://hz.cucudq.cn/gterrtjhek.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.dianchejie.cn/gtgbowtsvy.html

[S55] C++：结构化绑定
来源：http://hz.ppjwa.cn/gtgbxnthuj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.smart0.xyz/gtcjlofugq.html

[S56] C++：optional
来源：http://hz.gotoacloud.top/gtubkqttmj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.hysaishi.cn/gtllrnegvt.html

[S57] C++：编译期常量
来源：http://hz.ydzc1.top/gtyafzzbwq.html

constexpr int N = 10;
来源：http://hz.ybcxt.top/gteigfezba.html

[S58] C++：命名空间
来源：http://hz.jiagoushi.top/gtjcbdpidq.html

namespace ns { int f() { return 1; } }
来源：http://hz.0kj1m.cn/gtjwjkdqlq.html

[S59] C++：静态断言
来源：http://hz.cdnleiting.top/gtwgnspkmb.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hammf.cn/gtfiypmxxe.html

[S60] C++：遍历并删除元素
来源：http://hz.hongshengwenyu.top/gtydxsdrew.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.quarkkingdee.top/gttnyboiac.html

================================================================================
来源：http://hz.52xcode.cn/gtejcyjoze.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhaomingkeji.xyz/gtfbdjsjmm.html

================================================================================
来源：http://hz.bjfxy.top/gtmaxkcjmj.html

[T01] Kotlin：Hello World
来源：http://hz.xziqi.cn/gtzimjczed.html

println("Hello")
来源：http://hz.haohaochexian.top/gtzeviuzwa.html

[T02] Kotlin：变量
来源：http://hz.hammf.cn/gtlmdfavob.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.hnqzz.top/gtfwbnmkuu.html

[T03] Kotlin：字符串模板
来源：http://hz.shuidangran.top/gtfbhjshwk.html

"值: $b"
来源：http://hz.zhongyouzk.top/gtwepeibyx.html

[T04] Kotlin：空安全
来源：http://hz.fzhhl.top/gtvtudhchd.html

val n: String? = null;  n?.length
来源：http://hz.shuidangran.top/gtaoudvonp.html

[T05] Kotlin：when 表达式
来源：http://hz.smart0.xyz/gtevmxbztr.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xingfuxueyuan.xyz/gtrhxtaaeb.html

[T06] Kotlin：集合映射
来源：http://hz.kuanghao11.cn/gtnphmjvmn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.sysykeji.top/gtqouqbpdd.html

[T07] Kotlin：集合过滤
来源：http://hz.316326.xyz/gtopzxnrwc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.shuidangran.top/gttmymrode.html

[T08] Kotlin：数据类
来源：http://hz.fengsongda.top/gtmenqdoml.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtslzsnucq.html

[T09] Kotlin：扩展函数
来源：http://hz.quarkkingdee.top/gtrckldpsp.html

fun String.exclaim() = this + "!"
来源：http://hz.9152youxi.cn/gtahokxmls.html

[T10] Kotlin：默认参数
来源：http://hz.wangdashe.top/gtufkcqgyv.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.andypj.xyz/gtifkfjqtl.html

[T11] Kotlin：协程
来源：http://hz.aibaodan.cn/gtyjyeevbs.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.cqqwz.cn/gtyhooxasy.html

[T12] Kotlin：解构声明
来源：http://hz.ydzc1.top/gtrgkmqwlt.html

val (a, b) = Pair(1, 2)
来源：http://hz.ppjwa.cn/gtmkhghdnp.html

[T13] Kotlin：只读 Map
来源：http://hz.nwbrower.top/gtfpcbwdsz.html

val m = mapOf("a" to 1)
来源：http://hz.316326.xyz/gtsqwmeqan.html

[T14] Kotlin：循环
来源：http://hz.zdqjudy.top/gtkjvdzcei.html

for (i in 1..10) println(i)
来源：http://hz.pengpengdd.cyou/gtzvmtqigv.html

[T15] Kotlin：接口
来源：http://hz.xingfuxueyuan.xyz/gtuteqmgcs.html

interface Shape { fun area(): Double }
来源：http://hz.nwbrower.top/gtchljmbgq.html

[T16] Swift：Hello World
来源：http://hz.aizwys.cn/gtlfuqnowd.html

print("Hello")
来源：http://hz.ppjwa.cn/gtnbqxjtzx.html

[T17] Swift：变量与常量
来源：http://hz.havefunace.top/gtkbqdvuwz.html

var a = 1;  let b = 2
来源：http://hz.zhaomingkeji.xyz/gtbkjladph.html

[T18] Swift：字符串插值
来源：http://hz.meibo888.top/gtjgavtnsu.html

"值: \(b)"
来源：http://hz.jiagoushi.top/gtldjefaas.html

[T19] Swift：可选绑定
来源：http://hz.xuetiantiany.cn/gtjfdejick.html

if let n = opt { print(n) }
来源：http://hz.yvedp.cn/gtpvdersnu.html

[T20] Swift：数组操作
来源：http://hz.shzxlz.cn/gtiogumzda.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.wangdashe.top/gtwcwwdccm.html

[T21] Swift：遍历
来源：http://hz.gzhubu.top/gtxqhgcnrm.html

for x in a { print(x) }
来源：http://hz.svipenyu.cn/gtktuovpde.html

[T22] Swift：字典
来源：http://hz.0kj1m.cn/gtuwvbfbrr.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.gotoacloud.top/gtqisplugj.html


<!-- 参考信息 -->