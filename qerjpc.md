代发 wailian999

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hongshengwenyu.top/gtzfylqree.html

[R18] 遍历数组
来源：http://hz.tianlin.xyz/gtfayylowi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.0kj1m.cn/gtrqcjkbie.html

[R19] 数组长度
来源：http://hz.zhoulong.xyz/gtpbkycwqi.html

echo "${#arr[@]}"
来源：http://hz.gaohongyu789.top/gttaqpntsh.html

[R20] 关联数组（字典）
来源：http://hz.xuanzx.com/gtmksplbbu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxinkj.top/gtxfaycvqr.html

[R21] 字符串长度
来源：http://hz.gzhubu.top/gtvlnmxdiw.html

echo "${#s}"
来源：http://hz.yuanzhike.top/gtcnptpfwp.html

[R22] 截取子串
来源：http://hz.yj20258888.top/gtgvmuitpb.html

echo "${s:0:5}"
来源：http://hz.ehwqpu.com/gtqyejseuo.html

[R23] 字符串替换
来源：http://hz.yj20258888.top/gttghsylyb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xuetiantiany.cn/gteobvjpjz.html

[R24] 大小写转换
来源：http://hz.zhiwuduotai.top/gtyjrtnzuc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hysaishi.cn/gtmcsyvojs.html

[R25] 去后缀 / 去前缀
来源：http://hz.hywenlv.cn/gtilkmxoor.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yvedp.cn/gtxrlexnub.html

[R26] 命令替换
来源：http://hz.guannengcc.top/gtluixqgsx.html

now=$(date +%F); echo "$now"
来源：http://hz.snrcjt.cn/gthxjrmkzy.html

[R27] 算术展开
来源：http://hz.daria6918.cn/gtzeinueed.html

echo $((1 + 2 * 3))
来源：http://hz.xuanzx.com/gtelfcbghd.html

[R28] 浮点运算
来源：http://hz.shuidangran.top/gtzjmpfkhm.html

echo "scale=2; 10/3" | bc
来源：http://hz.yongpay.top/gtimkbziuq.html

[R29] 定义函数
来源：http://hz.ppjwa.cn/gtkehpxmrb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yonumen.top/gtfpgulajz.html

[R30] 函数返回状态码
来源：http://hz.gzhubu.top/gtwleobjud.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hnqzz.top/gtwowcxycd.html

[R31] 局部变量
来源：http://hz.yangfankeji.com/gthmudrahv.html

f() { local x=1; echo "$x"; }
来源：http://hz.sufxvd.cn/gtgfyjuuzp.html

[R32] 参数个数校验
来源：http://hz.xinyue.icu/gtjevslisj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.cdnleiting.top/gtjhzhiclh.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtqzbbiuuh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.pengpengdd.cyou/gtariywagd.html

[R34] 退出时清理
来源：http://hz.hnqzz.top/gtultklyay.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhoulong.xyz/gtdkpcegkb.html

[R35] 后台执行并等待
来源：http://hz.sysykeji.top/gtbjzdbwyf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.meibo888.top/gtwvcijhyt.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtxghgzdkc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.hnqzz.top/gttyqmltfw.html

[R37] 把输出赋给变量
来源：http://hz.smart0.xyz/gtdfxvsoun.html

files=$(ls -1)
来源：http://hz.9152youxi.cn/gtflxrerms.html

[R38] 管道串联
来源：http://hz.redwolf501.top/gtzzlutfxi.html

cat a.txt | grep -i error | wc -l
来源：http://hz.iojbl.cn/gtzoyjpjxj.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtunqlhgot.html

cmd > out.log 2>&1
来源：http://hz.shuidangran.top/gtiwooxbln.html

[R40] 追加写日志
来源：http://hz.chenzaomai.com/gtxbmzqsdh.html

echo "log" >> out.log
来源：http://hz.yj20258.top/gtqgrjqcfq.html

[R41] 丢弃输出
来源：http://hz.dianchejie.cn/gtkmfbjwpi.html

cmd >/dev/null 2>&1
来源：http://hz.ydjk.org.cn/gtftmquqrx.html

[R42] 输入重定向
来源：http://hz.quarkkingdee.top/gtvfnoixxl.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtqigdcjgs.html

[R43] 按名字查找文件
来源：http://hz.nanxuanxn.top/gtvskcgzkc.html

find . -name "*.log" -type f
来源：http://hz.sufxvd.cn/gtazycdjwx.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtdswjekcz.html

find . -mtime -7 -type f
来源：http://hz.hnqzz.top/gtogydwemh.html

[R45] 批量删除
来源：http://hz.redwolf501.top/gtvifrvgip.html

find . -name "*.tmp" -delete
来源：http://hz.jianghu66.top/gtmctiygst.html

[R46] 递归替换文件内容
来源：http://hz.hfpthk.cn/gtbrfeidta.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shangyingyoupin.top/gtfsuqlitv.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtihdplniu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigfzy.top/gtyphcyljq.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtoeekjwge.html

awk '{print $1, $3}' a.txt
来源：http://hz.iojbl.cn/gtxasqwiwa.html

[R49] awk 带条件
来源：http://hz.hammf.cn/gtdlhktbda.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.sxryk.cn/gtzqcdvxrg.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtgxcncftz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinqigufen.top/gtbqyhfsfk.html

[R51] 排序去重取前几
来源：http://hz.ehwqpu.com/gtjzuhfltk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinghuilouyu.cn/gtlouyxarh.html

[R52] 统计行数
来源：http://hz.zhongyouzk.top/gtwoinclhd.html

wc -l a.txt
来源：http://hz.dashuyun.cn/gtpifrbtdd.html

[R53] 查看文件头与实时尾
来源：http://hz.pycfn.com/gtfiflydzs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtunckoazq.html

[R54] 比较两个文件
来源：http://hz.smart0.xyz/gtuehldojq.html

diff a.txt b.txt
来源：http://hz.jyoumei.cn/gtgieoodrr.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtyrvggpwv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinqigfzy.top/gtvlsfuecj.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gttmlhmdna.html

scp file user@host:/path/
来源：http://hz.hfpthk.cn/gtfakkwaqa.html

[R57] 远程执行命令
来源：http://hz.hongshengwenyu.top/gtmvhhrhhk.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtvffnecsj.html

[R58] 下载文件
来源：http://hz.fzhhl.top/gtypsrlvfg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtcwoeoona.html

[R59] 发 POST JSON
来源：http://hz.zhijiandao.cn/gtxalrxfik.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zdqjudy.top/gtsnfkuabc.html

[R60] 只看 HTTP 状态码
来源：http://hz.hnxiangtu.top/gtfhjoevic.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtkvvjuygi.html

[R61] 磁盘占用
来源：http://hz.gogol.net.cn/gtvjgbluok.html

df -h;  du -sh *
来源：http://hz.shanyushiyangtech.top/gtraokzcli.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gthrbsdtco.html

du -ah . | sort -rh | head -10
来源：http://hz.yangfankeji.com/gtscrlxwhm.html

[R63] 内存与进程
来源：http://hz.cashguo.top/gtmxszqwjq.html

free -h;  ps aux | grep nginx
来源：http://hz.yanxiufei.cn/gtcurckrcy.html

[R64] 结束进程
来源：http://hz.gzhubu.top/gtnxekthui.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yueranfly.top/gtsuqrdkit.html

[R65] 查看端口占用
来源：http://hz.9152youxi.cn/gtihdaxouh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtpgkbqvog.html

[R66] 定时任务
来源：http://hz.guowangkeji.top/gtnfarhibg.html

crontab -e;  crontab -l
来源：http://hz.zhengqikj.top/gtnsyqewtu.html

[R67] 生成随机十六进制串
来源：http://hz.bjfxy.top/gttkzbmvqj.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gtwkkhbtqn.html

[R68] 计算文件校验值
来源：http://hz.jinqigfzy.top/gtxerysmmu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtvizkklvt.html

[R69] 生成随机密码
来源：http://hz.cdnleiting.top/gtpuxutxwo.html

head -c 16 /dev/urandom | base64
来源：http://hz.zhongyouzk.top/gtwjqoyubq.html

[R70] 时间戳与互转
来源：http://hz.ivvv.top/gtdnzaehhk.html

date +%s;  date -d @1700000000
来源：http://hz.9152youxi.cn/gtyhvbhfqr.html

[R71] 日期格式化
来源：http://hz.daxiang520.top/gtpmcogdvb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zhoulong.xyz/gtfmjbuekx.html

[R72] 等待端口就绪
来源：http://hz.zhengqikj.top/gtvswtynyz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtwbvkuptq.html

[R73] 分割大日志
来源：http://hz.aibaodan.cn/gtjkiybscz.html

split -l 1000 big.log part_
来源：http://hz.dianchejie.cn/gtbejvkchh.html

[R74] 批量重命名
来源：http://hz.aibaodan.cn/gtazbguiin.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hysaishi.cn/gttvpxrclt.html

[R75] 导出环境变量
来源：http://hz.316326.xyz/gtgjcsfips.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yvedp.cn/gtcgpafawh.html

[R76] 使用临时文件
来源：http://hz.ybcxt.top/gtvlmihdtp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.mhx1999.top/gtrbcuqsph.html

[R77] 读取用户输入
来源：http://hz.jqgufenzy.top/gtwwfaaxbf.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gtjslyvikt.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gthkfpkbyv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.daxiang520.top/gtiuwnatlk.html

[R79] 解析命令行选项
来源：http://hz.sweek.top/gtlzaiphdr.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gtgvykylhd.html

[R80] 查看脚本执行耗时
来源：http://hz.zhijiandao.cn/gtvbkyjbyr.html

time ./run.sh
来源：http://hz.cdnleiting.top/gtcyarvyli.html

================================================================================
来源：http://hz.yueranfly.top/gtrasxmhwr.html

S. C / C++ 专题
来源：http://hz.gaohongyu789.top/gtzayajenv.html

================================================================================
来源：http://hz.yuxming.cn/gtnswbrmfo.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtcuwdeewb.html

#include <stdio.h>
来源：http://hz.hnxiangtu.top/gtwifnspbx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jianghu66.top/gtejlfxzqm.html

[S02] C：变量与格式化输出
来源：http://hz.aibaodan.cn/gtzirycvgv.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtnlycsdms.html

[S03] C：读入整数
来源：http://hz.c1oappe.top/gthlezbebj.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtitohsvmt.html

[S04] C：字符串复制
来源：http://hz.smart0.xyz/gtkjuygmxv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinyuanbaomall.cn/gtkkolpgwb.html

[S05] C：字符串长度
来源：http://hz.yonumen.top/gtdhfrdllu.html

strlen(s)
来源：http://hz.xuanzx.com/gtuetlagsb.html

[S06] C：字符串比较
来源：http://hz.chenlongwang.top/gtxhyzlfts.html

strcmp(a, b) == 0
来源：http://hz.sysykeji.top/gtubvmrvig.html

[S07] C：数组遍历求和
来源：http://hz.shuidangran.top/gtftclvcld.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.fzhhl.top/gthxmejhxk.html

[S08] C：动态内存分配与释放
来源：http://hz.aizwys.cn/gtbncmyolp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtjbntkieb.html

[S09] C：结构体定义与初始化
来源：http://hz.shzxlz.cn/gtfckdhprq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gtkihdspxx.html

[S10] C：指针与解引用
来源：http://hz.shanyushiyangtech.top/gtxbkkycje.html

int *p = &a;  *p = 5;
来源：http://hz.gotoacloud.top/gtsxqdkuan.html

[S11] C：逐行读文件
来源：http://hz.aibaodan.cn/gtbrhktqfo.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hongshengwenyu.top/gtryfilins.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.gzhubu.top/gtexnjunfa.html

fclose(f);
来源：http://hz.cqqwz.cn/gtpbusapnx.html

[S12] C：写文件
来源：http://hz.sysykeji.top/gttorsfoik.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtcumjmooh.html

[S13] C：宏定义
来源：http://hz.shangyingyoupin.top/gtugaitlvu.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.52xcode.cn/gtfybgtzfp.html

[S14] C：枚举
来源：http://hz.yuanzhike.top/gtkynpjchv.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aizwys.cn/gtxkunybwm.html

[S15] C：类型转换
来源：http://hz.jqgufenzy.top/gtfllwhzvt.html

(double) a / b
来源：http://hz.sufxvd.cn/gtrvwfjspz.html

[S16] C：位操作置位
来源：http://hz.dianchejie.cn/gtvkgxyuwr.html

x |= (1 << 3);
来源：http://hz.hongshengwenyu.top/gtyvdnjuez.html

[S17] C：安全拼接字符串
来源：http://hz.pycfn.com/gtovznwsyp.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.fengsongda.top/gtxqbdknnl.html

[S18] C：命令行参数
来源：http://hz.ydjk.org.cn/gttwkxnyak.html

int main(int argc, char **argv)
来源：http://hz.jqgfzy.top/gtpomtoekl.html

[S19] C：快速排序
来源：http://hz.shzxlz.cn/gtqxkhnjjt.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtssfrobcb.html

[S20] C：二分查找
来源：http://hz.xinyue.icu/gtuctqmmba.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.bjfxy.top/gtmnzzgcvu.html

[S21] C：字符类别判断
来源：http://hz.cheryme.top/gtfwdgvcin.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.havefunace.top/gtfofqdauu.html

[S22] C：字符串转数字
来源：http://hz.redwolf501.top/gtsqxtmqvg.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.ivvv.top/gtmaeyapnj.html

[S23] C：随机数
来源：http://hz.guannengcc.top/gtjfezrvos.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jinqigfzy.top/gtfskzwjsm.html

[S24] C：获取本地时间
来源：http://hz.ehwqpu.com/gtncvspjnu.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yuxming.cn/gtjvmjqeal.html

[S25] C：内存拷贝
来源：http://hz.cashguo.top/gtycjvvovb.html

memcpy(dst, src, n);
来源：http://hz.hysaishi.cn/gtafrdmkjg.html

[S26] C：内存清零
来源：http://hz.wangshuangyany.cn/gtanywqgwd.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtnovwvord.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtpzwizatz.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtwndnfrkd.html

[S28] C：静态变量
来源：http://hz.daxiang520.top/gtdbvnkxwv.html

static int counter = 0;
来源：http://hz.sxryk.cn/gtgqpvdomg.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gtewunvqzr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.chenjidiqi.icu/gtaxlqqyom.html

[S30] C：头文件保护
来源：http://hz.shzxlz.cn/gteulcktck.html

#ifndef X_H
来源：http://hz.ydjk.org.cn/gtukyqoehd.html

#define X_H
来源：http://hz.sysykeji.top/gtshagljok.html

#endif
来源：http://hz.meibo888.top/gtbwpiygll.html

[S31] C++：Hello World
来源：http://hz.jqgufenzy.top/gtcjnxwojc.html

#include <iostream>
来源：http://hz.fzhhl.top/gtzemykcks.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zhongyouzk.top/gtludxzskw.html

[S32] C++：字符串
来源：http://hz.jinqigufen.top/gtlgjfslem.html

std::string s = "hi";  s += "!";
来源：http://hz.zhengqikj.top/gtpzidctoq.html

[S33] C++：vector 增删
来源：http://hz.ydzc1.top/gtmuggysjo.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.sweek.top/gtltgscyab.html

[S34] C++：遍历 vector
来源：http://hz.xuanzx.com/gtawythzsa.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yvedp.cn/gtqsrpprlx.html

[S35] C++：map
来源：http://hz.hnxiangtu.top/gtvltkjawp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tianlin.xyz/gtoubndqoc.html

[S36] C++：unordered_map
来源：http://hz.cashguo.top/gtvhtjbpio.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenlongwang.top/gtayopzxsq.html

[S37] C++：set
来源：http://hz.sxryk.cn/gtxqrddwbd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhaomingkeji.xyz/gtwmfxuaro.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtdfomgqtk.html

std::sort(v.begin(), v.end());
来源：http://hz.9152youxi.cn/gtojhfolzm.html

[S39] C++：自定义比较器排序
来源：http://hz.xuanzx.com/gtxaaiyolx.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.kuanghao11.cn/gtzeriejaj.html

[S40] C++：查找元素
来源：http://hz.ivvv.top/gtfeachata.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.dashuyun.cn/gtmxvdzqjn.html

[S41] C++：类与构造函数
来源：http://hz.tanke756.top/gtnngkbxdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gtfmubyyie.html

[S42] C++：继承与虚函数
来源：http://hz.tianlin.xyz/gtrzyxiehi.html

class B : public Base { public: void f() override {} };
来源：http://hz.ybcxt.top/gtpinryabi.html

[S43] C++：智能指针
来源：http://hz.haohaochexian.top/gtkpvtosrh.html

auto p = std::make_unique<int>(5);
来源：http://hz.guowangkeji.top/gtgxyutsfb.html

[S44] C++：引用传参
来源：http://hz.aizwys.cn/gtnksfcwwy.html

void inc(int &x) { ++x; }
来源：http://hz.gogol.net.cn/gtzfwfqsrs.html

[S45] C++：lambda
来源：http://hz.dashuyun.cn/gtxuaczija.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yuxming.cn/gtjqflqtxx.html

[S46] C++：函数模板
来源：http://hz.guowangkeji.top/gtglsrydke.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.kuanghao11.cn/gtaxctfzll.html

[S47] C++：结构化绑定遍历
来源：http://hz.yvedp.cn/gtwzjaotjv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.mhx1999.top/gtxfensfoh.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtceguoseg.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zycfv.cn/gtnqkzhbvs.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258888.top/gtfcsbrrei.html

[S49] C++：写文件
来源：http://hz.daxiang520.top/gtixsplaar.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.daria6918.cn/gtzugiypbg.html

[S50] C++：格式化数字
来源：http://hz.jinqigfzy.top/gtnsvzfoqm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtobkpxwip.html

[S51] C++：显式类型转换
来源：http://hz.yvedp.cn/gtbuzainbx.html

static_cast<double>(a) / b
来源：http://hz.birdmap.top/gtmimwycuz.html

[S52] C++：const 与 noexcept
来源：http://hz.snrcjt.cn/gthbymsstk.html

int size() const noexcept { return n_; }
来源：http://hz.yangfankeji.com/gtffkjmadh.html

[S53] C++：移动语义
来源：http://hz.chenlongwang.top/gtwwmuknxg.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigufen.top/gttdnisvpx.html

[S54] C++：异常处理
来源：http://hz.tianlin.xyz/gtmrnyaobv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxuanxn.top/gtpcueemhz.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gtgexmyxhk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yonumen.top/gttycyjotc.html

[S56] C++：optional
来源：http://hz.gogol.net.cn/gtsnszcucl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.chenzaomai.com/gtoenqtlnb.html

[S57] C++：编译期常量
来源：http://hz.sweek.top/gttbbxrzqy.html

constexpr int N = 10;
来源：http://hz.pycfn.com/gtuuldaape.html

[S58] C++：命名空间
来源：http://hz.svipenyu.cn/gtsmawpjlz.html

namespace ns { int f() { return 1; } }
来源：http://hz.jianghu66.top/gtrczourhj.html

[S59] C++：静态断言
来源：http://hz.fengsongda.top/gtpjowehju.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.smart0.xyz/gtcnzuicxg.html

[S60] C++：遍历并删除元素
来源：http://hz.ehwqpu.com/gtyreqymjd.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shangyingyoupin.top/gtpmzmvpdq.html

================================================================================
来源：http://hz.sysykeji.top/gtcxbozghs.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.shzxlz.cn/gtduxkqdhc.html

================================================================================
来源：http://hz.pengpengdd.cyou/gttioylraq.html

[T01] Kotlin：Hello World
来源：http://hz.pengpengdd.cyou/gtwlaaichd.html

println("Hello")
来源：http://hz.dianchejie.cn/gtdaqzasgo.html

[T02] Kotlin：变量
来源：http://hz.gaohongyu789.top/gtxvrqimbm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.vqdsnc.cn/gtdnkkxdst.html

[T03] Kotlin：字符串模板
来源：http://hz.jqgufenzy.top/gtxcvetngh.html

"值: $b"
来源：http://hz.yuxming.cn/gtanviwluz.html

[T04] Kotlin：空安全
来源：http://hz.ydjk.org.cn/gtuqnikbam.html

val n: String? = null;  n?.length
来源：http://hz.yangfankeji.com/gtpyvatkkx.html

[T05] Kotlin：when 表达式
来源：http://hz.dashuyun.cn/gtpopmofaw.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hfpthk.cn/gtqnwjsikg.html

[T06] Kotlin：集合映射
来源：http://hz.yuxming.cn/gtlbkstoje.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.gzhubu.top/gttewwcvrw.html

[T07] Kotlin：集合过滤
来源：http://hz.zhongyouzk.top/gtchcpiure.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.jyoumei.cn/gtqzwtbign.html

[T08] Kotlin：数据类
来源：http://hz.jianghu66.top/gtudqywzbe.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtfsbccmcf.html

[T09] Kotlin：扩展函数
来源：http://hz.smart0.xyz/gtmeovjrbb.html

fun String.exclaim() = this + "!"
来源：http://hz.cashguo.top/gtshieajfp.html

[T10] Kotlin：默认参数
来源：http://hz.snrcjt.cn/gtshgmgvld.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xylfe.cn/gtledfrflc.html

[T11] Kotlin：协程
来源：http://hz.9152youxi.cn/gtipkkiyma.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.ybcxt.top/gtzfttrwoz.html

[T12] Kotlin：解构声明
来源：http://hz.iojbl.cn/gtwmcaviqn.html

val (a, b) = Pair(1, 2)
来源：http://hz.xylfe.cn/gtiyjxrovw.html

[T13] Kotlin：只读 Map
来源：http://hz.ppjwa.cn/gtqvyxdxum.html

val m = mapOf("a" to 1)
来源：http://hz.quarkkingdee.top/gtewmuldls.html

[T14] Kotlin：循环
来源：http://hz.aizwys.cn/gtpxqbwplf.html

for (i in 1..10) println(i)
来源：http://hz.hywenlv.cn/gtnrqtqdhk.html

[T15] Kotlin：接口
来源：http://hz.zhongyouzk.top/gtpvfbhpio.html

interface Shape { fun area(): Double }
来源：http://hz.shanyushiyangtech.top/gttdmmcyyr.html

[T16] Swift：Hello World
来源：http://hz.gzhubu.top/gtkwfnrkbq.html

print("Hello")
来源：http://hz.ydzc1.top/gtvayuttmz.html

[T17] Swift：变量与常量
来源：http://hz.haohaochexian.top/gtrdsdlwju.html

var a = 1;  let b = 2
来源：http://hz.hammf.cn/gtczugjphz.html

[T18] Swift：字符串插值
来源：http://hz.sufxvd.cn/gtdzddhhdi.html

"值: \(b)"
来源：http://hz.dianchejie.cn/gthgoqzedr.html

[T19] Swift：可选绑定
来源：http://hz.smart0.xyz/gtzugkcvjv.html

if let n = opt { print(n) }
来源：http://hz.shanyushiyangkeji.top/gteptkbkbw.html

[T20] Swift：数组操作
来源：http://hz.c1oappe.top/gtpktfgxql.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangtech.top/gtsykcvcjr.html


<!-- 参考信息 -->