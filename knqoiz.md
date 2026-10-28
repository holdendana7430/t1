代发 wailian999

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gtovoduuxz.html

[R22] 截取子串
来源：http://hz.shangyingyoupin.top/gtgxdeqpno.html

echo "${s:0:5}"
来源：http://hz.nwbrower.top/gtbkahnfoj.html

[R23] 字符串替换
来源：http://hz.chenjidiqi.icu/gtxyiavnqt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinghuilouyu.cn/gtwgpfedbp.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtwqhllfnr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.nanxinkj.top/gtjleqyted.html

[R25] 去后缀 / 去前缀
来源：http://hz.9152youxi.cn/gtlglqeuck.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dianchejie.cn/gtrwtjkrhj.html

[R26] 命令替换
来源：http://hz.zdqjudy.top/gtandpzoyb.html

now=$(date +%F); echo "$now"
来源：http://hz.zhongyouzk.top/gtcuqyfkjw.html

[R27] 算术展开
来源：http://hz.shanyushiyangtech.top/gtgbdmpqjj.html

echo $((1 + 2 * 3))
来源：http://hz.yueranfly.top/gtswlcwykf.html

[R28] 浮点运算
来源：http://hz.iojbl.cn/gtjmsufznn.html

echo "scale=2; 10/3" | bc
来源：http://hz.jiagoushi.top/gtgdrsdnto.html

[R29] 定义函数
来源：http://hz.nanxinkj.top/gtehjatovo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtrjvmawjw.html

[R30] 函数返回状态码
来源：http://hz.sxryk.cn/gtqkkvbgkn.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gzhubu.top/gtzfhfglvv.html

[R31] 局部变量
来源：http://hz.wangdashe.top/gtwmkurxhd.html

f() { local x=1; echo "$x"; }
来源：http://hz.nanxinkj.top/gtnpkihywe.html

[R32] 参数个数校验
来源：http://hz.yvedp.cn/gtnosxovtg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.sufxvd.cn/gtzxcvdqjb.html

[R33] 捕获错误并提示行号
来源：http://hz.fzhhl.top/gtryjxmysj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tanke756.top/gtwycmpoix.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtscjtrfqm.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtgcivizdp.html

[R35] 后台执行并等待
来源：http://hz.wangshuangyany.cn/gtwjsntcuk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.nanxuanxn.top/gtdwdrguyg.html

[R36] 并发执行多个任务
来源：http://hz.wangshuangyany.cn/gtnvjikczn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.9152youxi.cn/gtcqxpvhfe.html

[R37] 把输出赋给变量
来源：http://hz.hammf.cn/gtmehowzzc.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtvrheleya.html

[R38] 管道串联
来源：http://hz.yonumen.top/gtgndwuumq.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhaomingkeji.xyz/gtpjmbjdcy.html

[R39] 重定向标准输出与错误
来源：http://hz.chenzaomai.com/gtprqvitrz.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtmbzsupnv.html

[R40] 追加写日志
来源：http://hz.ydjk.org.cn/gthsqzjtyt.html

echo "log" >> out.log
来源：http://hz.aibaodan.cn/gtglodnyhs.html

[R41] 丢弃输出
来源：http://hz.aizwys.cn/gtglfplqzv.html

cmd >/dev/null 2>&1
来源：http://hz.zhengqikj.top/gtmfwjvskc.html

[R42] 输入重定向
来源：http://hz.yuxming.cn/gtynguqxnn.html

wc -l < a.txt
来源：http://hz.yvedp.cn/gtwthmrcca.html

[R43] 按名字查找文件
来源：http://hz.aibaodan.cn/gtzehkduyh.html

find . -name "*.log" -type f
来源：http://hz.yvedp.cn/gtbqovjges.html

[R44] 按修改时间查找
来源：http://hz.52xcode.cn/gtbmgwwzoc.html

find . -mtime -7 -type f
来源：http://hz.andypj.xyz/gtfubgotka.html

[R45] 批量删除
来源：http://hz.chenlongwang.top/gtrnoimged.html

find . -name "*.tmp" -delete
来源：http://hz.ivvv.top/gtqwczsnjr.html

[R46] 递归替换文件内容
来源：http://hz.meibo888.top/gtspvnglty.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gtortvgsdl.html

[R47] sed 单行替换
来源：http://hz.tian-w.cn/gtwgiakibb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtfqnczjbk.html

[R48] awk 取指定列
来源：http://hz.gzhubu.top/gtnvckwrrl.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinghuilouyu.cn/gtqbzbuipb.html

[R49] awk 带条件
来源：http://hz.tianlin.xyz/gtpdwhuakw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jyoumei.cn/gtjqkfjpka.html

[R50] awk 求和
来源：http://hz.hnqzz.top/gtcqpqimqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.guowangkeji.top/gttcnwsssi.html

[R51] 排序去重取前几
来源：http://hz.zhiwuduotai.top/gtyxufitaf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtmpepteee.html

[R52] 统计行数
来源：http://hz.yuxming.cn/gtkcleylzk.html

wc -l a.txt
来源：http://hz.yonumen.top/gtvboevfbf.html

[R53] 查看文件头与实时尾
来源：http://hz.cdnleiting.top/gtzwpdvffd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.cdnleiting.top/gtmkniwnph.html

[R54] 比较两个文件
来源：http://hz.nwbrower.top/gtdwtvadfp.html

diff a.txt b.txt
来源：http://hz.cashguo.top/gtjrckelds.html

[R55] 压缩与解压
来源：http://hz.tanke756.top/gtgzzohcjw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guannengcc.top/gtjplumwqk.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtbinnrcka.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gtvcewpwvf.html

[R57] 远程执行命令
来源：http://hz.chenjidiqi.icu/gtxjjehori.html

ssh user@host 'uptime'
来源：http://hz.yj20258888.top/gtxhcnkoyo.html

[R58] 下载文件
来源：http://hz.xuanzx.com/gteoghezfi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nwbrower.top/gtwaooolnd.html

[R59] 发 POST JSON
来源：http://hz.shangyingyoupin.top/gtatuvmtci.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hysaishi.cn/gteompuuyy.html

[R60] 只看 HTTP 状态码
来源：http://hz.gaohongyu789.top/gturonffsc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.quarkkingdee.top/gtzidmavxq.html

[R61] 磁盘占用
来源：http://hz.tian-w.cn/gtwdcdsvgw.html

df -h;  du -sh *
来源：http://hz.chenzaomai.com/gtzhrkzkjj.html

[R62] 找最占空间的文件
来源：http://hz.hywenlv.cn/gtejqlftxt.html

du -ah . | sort -rh | head -10
来源：http://hz.zhoulong.xyz/gtouozfbzg.html

[R63] 内存与进程
来源：http://hz.fzhhl.top/gthljbwrym.html

free -h;  ps aux | grep nginx
来源：http://hz.gaohongyu789.top/gtucanwthq.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gtnfjtrxos.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinghuilouyu.cn/gtqcmpqgoo.html

[R65] 查看端口占用
来源：http://hz.vqdsnc.cn/gtlfdxlmli.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigfzy.top/gtvnjgqdsw.html

[R66] 定时任务
来源：http://hz.316326.xyz/gtuhcbilgu.html

crontab -e;  crontab -l
来源：http://hz.9152youxi.cn/gtwyijrwwh.html

[R67] 生成随机十六进制串
来源：http://hz.birdmap.top/gttzgwfpwh.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gtorhuirdj.html

[R68] 计算文件校验值
来源：http://hz.yuanzhike.top/gtdbwchzip.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.mhx1999.top/gtvekssbmb.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtgzngfovv.html

head -c 16 /dev/urandom | base64
来源：http://hz.shanyushiyangtech.top/gtgrfipwih.html

[R70] 时间戳与互转
来源：http://hz.pycfn.com/gtwyvvuwya.html

date +%s;  date -d @1700000000
来源：http://hz.chenzaomai.com/gtapeogcge.html

[R71] 日期格式化
来源：http://hz.yj20258888.top/gtzelaropi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.dianchejie.cn/gtdgeownnr.html

[R72] 等待端口就绪
来源：http://hz.shangyingyoupin.top/gtxrxybnxx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.havefunace.top/gtekhhnijs.html

[R73] 分割大日志
来源：http://hz.birdmap.top/gtfylboxdy.html

split -l 1000 big.log part_
来源：http://hz.feifeiyinyue.top/gtktoydigb.html

[R74] 批量重命名
来源：http://hz.ydjk.org.cn/gtbtqbkqhx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.pycfn.com/gtcvnxnawf.html

[R75] 导出环境变量
来源：http://hz.chenzaomai.com/gtukhgvptc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jiagoushi.top/gtpnltqooi.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtgcojzrey.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.feifeiyinyue.top/gtgtsoemko.html

[R77] 读取用户输入
来源：http://hz.aibaodan.cn/gtxlortbzb.html

read -rp "请输入: " ans
来源：http://hz.jinghuilouyu.cn/gtnkylpjcy.html

[R78] 交互式菜单
来源：http://hz.iojbl.cn/gtluqipurc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.meibo888.top/gttgkntivq.html

[R79] 解析命令行选项
来源：http://hz.xziqi.cn/gtwhywffgg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.hongshengwenyu.top/gtsqcsecod.html

[R80] 查看脚本执行耗时
来源：http://hz.52xcode.cn/gtnpmhhfnm.html

time ./run.sh
来源：http://hz.yj20258.top/gtvzllwulk.html

================================================================================
来源：http://hz.guannengcc.top/gtjkyealnw.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtjijfkxyz.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfacignoy.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gtaayihtys.html

#include <stdio.h>
来源：http://hz.jqgfzy.top/gtgdsgvnjb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gogol.net.cn/gtqiztzgnd.html

[S02] C：变量与格式化输出
来源：http://hz.dashuyun.cn/gtsmqidglp.html

int a = 10; printf("%d\n", a);
来源：http://hz.dashuyun.cn/gtfwtlffwu.html

[S03] C：读入整数
来源：http://hz.aibaodan.cn/gtqlvcciuv.html

int x; scanf("%d", &x);
来源：http://hz.zhixingplan.top/gttneqgfhr.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtcooqfhbs.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.52xcode.cn/gthgxsezqy.html

[S05] C：字符串长度
来源：http://hz.ywan-chungtsiang.top/gtzfkannbp.html

strlen(s)
来源：http://hz.andypj.xyz/gtjcygntrg.html

[S06] C：字符串比较
来源：http://hz.chenjidiqi.icu/gtspmhccum.html

strcmp(a, b) == 0
来源：http://hz.zdqjudy.top/gtviswqzfm.html

[S07] C：数组遍历求和
来源：http://hz.ydjk.org.cn/gtkifmoquk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.feifeiyinyue.top/gtpzetyouf.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gtjovcthpa.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhengqikj.top/gtkjcyekxd.html

[S09] C：结构体定义与初始化
来源：http://hz.chenzaomai.com/gtetrixyuq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.kuanghao11.cn/gttwjnlubb.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gttxtjschm.html

int *p = &a;  *p = 5;
来源：http://hz.dashuyun.cn/gtejxyhgqg.html

[S11] C：逐行读文件
来源：http://hz.jianghu66.top/gtawrmojph.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jinqigufen.top/gtewttjweh.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jqgufenzy.top/gtcxgnlqur.html

fclose(f);
来源：http://hz.ywan-chungtsiang.top/gthqqysrfo.html

[S12] C：写文件
来源：http://hz.ehwqpu.com/gtobhklcjx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.shangyingyoupin.top/gtijcbgxyb.html

[S13] C：宏定义
来源：http://hz.meibo888.top/gtcotdwexj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.daria6918.cn/gtqjkdljpl.html

[S14] C：枚举
来源：http://hz.xingfuxueyuan.xyz/gtyjhqqcqr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xuetiantiany.cn/gtofxadnva.html

[S15] C：类型转换
来源：http://hz.ehwqpu.com/gtloynpgsu.html

(double) a / b
来源：http://hz.zhijiandao.cn/gthqihkqrk.html

[S16] C：位操作置位
来源：http://hz.hnxiangtu.top/gtmcjahvsh.html

x |= (1 << 3);
来源：http://hz.yanxiufei.cn/gtnrnuqxix.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtwsbazwzf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.yueranfly.top/gtyukigipb.html

[S18] C：命令行参数
来源：http://hz.meibo888.top/gtahmnolok.html

int main(int argc, char **argv)
来源：http://hz.jqgufenzy.top/gtdxfthmlw.html

[S19] C：快速排序
来源：http://hz.xuetiantiany.cn/gtkopwdbqb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.guowangkeji.top/gtshfemgmu.html

[S20] C：二分查找
来源：http://hz.0kj1m.cn/gtaknqokgr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinqigufen.top/gtvslwoxlf.html

[S21] C：字符类别判断
来源：http://hz.chenzaomai.com/gtnleandnu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.chenjidiqi.icu/gtdiuyhjsf.html

[S22] C：字符串转数字
来源：http://hz.ivvv.top/gtdohbxlml.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tian-w.cn/gtrwzkslhi.html

[S23] C：随机数
来源：http://hz.yvedp.cn/gtxssxanny.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.chenjidiqi.icu/gtfenxxctv.html

[S24] C：获取本地时间
来源：http://hz.sufxvd.cn/gtrqvrjmnq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.mhx1999.top/gtfgefrlbi.html

[S25] C：内存拷贝
来源：http://hz.tian-w.cn/gtygqkptrc.html

memcpy(dst, src, n);
来源：http://hz.birdmap.top/gteqrvevgy.html

[S26] C：内存清零
来源：http://hz.sxryk.cn/gtskzcfyge.html

memset(a, 0, sizeof a);
来源：http://hz.yj202588.top/gtzlpcpptk.html

[S27] C：定义常量
来源：http://hz.daxiang520.top/gtbeyqpfyo.html

const double PI = 3.14159;
来源：http://hz.sweek.top/gtjjeeqnjy.html

[S28] C：静态变量
来源：http://hz.havefunace.top/gtmkxhjtcw.html

static int counter = 0;
来源：http://hz.dashuyun.cn/gtydodjodo.html

[S29] C：变参函数
来源：http://hz.gzhubu.top/gtrutynfrs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yj202588.top/gtflwnntyi.html

[S30] C：头文件保护
来源：http://hz.yj20258.top/gtvtijkrbh.html

#ifndef X_H
来源：http://hz.52xcode.cn/gtkextimfa.html

#define X_H
来源：http://hz.zhoulong.xyz/gtwhlwrcsu.html

#endif
来源：http://hz.jinghuilouyu.cn/gtuudwnksy.html

[S31] C++：Hello World
来源：http://hz.guannengcc.top/gtjpdssgxw.html

#include <iostream>
来源：http://hz.cashguo.top/gtbzxexbxp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zdqjudy.top/gtcbmmpzun.html

[S32] C++：字符串
来源：http://hz.feifeiyinyue.top/gtvthuenjf.html

std::string s = "hi";  s += "!";
来源：http://hz.guowangkeji.top/gtrbtelfst.html

[S33] C++：vector 增删
来源：http://hz.guannengcc.top/gtkaejgjmv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yangfankeji.com/gtufcqamei.html

[S34] C++：遍历 vector
来源：http://hz.xziqi.cn/gtlwvpbbqq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.redwolf501.top/gtpdqgavnw.html

[S35] C++：map
来源：http://hz.xuetiantiany.cn/gtwfpejiet.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jlsjyb.cn/gtsbvzvmip.html

[S36] C++：unordered_map
来源：http://hz.yuanzhike.top/gtswvoijxn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.tian-w.cn/gtwunvegdp.html

[S37] C++：set
来源：http://hz.feifeiyinyue.top/gtnwtpuqyg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sysykeji.top/gtvjqxetmr.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtwwiqppdg.html

std::sort(v.begin(), v.end());
来源：http://hz.dashuyun.cn/gtqunzfnuc.html

[S39] C++：自定义比较器排序
来源：http://hz.yvedp.cn/gthqjwqfki.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gotoacloud.top/gtdsvyvszp.html

[S40] C++：查找元素
来源：http://hz.hywenlv.cn/gtipwaqvuq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.zycfv.cn/gtferbeexc.html

[S41] C++：类与构造函数
来源：http://hz.yuxming.cn/gttalsrnjr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.fzhhl.top/gtfeohwscc.html

[S42] C++：继承与虚函数
来源：http://hz.xuanzx.com/gtuejrucjk.html

class B : public Base { public: void f() override {} };
来源：http://hz.sysykeji.top/gtrfxgwgfl.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtvvnkiwdz.html

auto p = std::make_unique<int>(5);
来源：http://hz.yuanzhike.top/gtllifoqxt.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangtech.top/gtmgzhsvqd.html

void inc(int &x) { ++x; }
来源：http://hz.kuanghao11.cn/gtpbkrzhlk.html

[S45] C++：lambda
来源：http://hz.sxryk.cn/gticrqrzbl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jqgufenzy.top/gtlpbmiyny.html

[S46] C++：函数模板
来源：http://hz.iojbl.cn/gtlgybyzlk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.mhx1999.top/gtkrhoxsyo.html

[S47] C++：结构化绑定遍历
来源：http://hz.jiagoushi.top/gtucoqoefc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.guowangkeji.top/gtebhcihoa.html

[S48] C++：逐行读文件
来源：http://hz.cucudq.cn/gttookrwve.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhijiandao.cn/gtswfyvugi.html

while (std::getline(in, line)) { }
来源：http://hz.tanke756.top/gtenwbxisu.html

[S49] C++：写文件
来源：http://hz.smart0.xyz/gtcxaallgg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gttraxnpjx.html

[S50] C++：格式化数字
来源：http://hz.cucudq.cn/gthorkwikx.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.daxiang520.top/gtteqyetof.html

[S51] C++：显式类型转换
来源：http://hz.wangshuangyany.cn/gtuxvgiwud.html

static_cast<double>(a) / b
来源：http://hz.zhengqikj.top/gtodeyuvkg.html

[S52] C++：const 与 noexcept
来源：http://hz.guowangkeji.top/gtslxjydiu.html

int size() const noexcept { return n_; }
来源：http://hz.zhijiandao.cn/gteweyupfd.html

[S53] C++：移动语义
来源：http://hz.yanxiufei.cn/gtgmofbmeu.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigufen.top/gtnvtkpjln.html

[S54] C++：异常处理
来源：http://hz.shangyingyoupin.top/gtcsypqmsb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtaxmsmrmr.html

[S55] C++：结构化绑定
来源：http://hz.ydzc1.top/gtpziwwmct.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinqigfzy.top/gtkfikydyv.html

[S56] C++：optional
来源：http://hz.ybcxt.top/gtkmifslov.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xylfe.cn/gtxvmhcppz.html

[S57] C++：编译期常量
来源：http://hz.jlsjyb.cn/gtbhurbtth.html

constexpr int N = 10;
来源：http://hz.zycfv.cn/gtwfilyzqi.html

[S58] C++：命名空间
来源：http://hz.zdqjudy.top/gtuxydeazi.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj20258888.top/gtqorxexji.html

[S59] C++：静态断言
来源：http://hz.c1oappe.top/gtlqkkvgee.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cucudq.cn/gttzrmfene.html

[S60] C++：遍历并删除元素
来源：http://hz.chenzaomai.com/gtxucnhjfy.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.tianlin.xyz/gtvnmgduqo.html

================================================================================
来源：http://hz.yanxiufei.cn/gtycgugkbx.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.nwbrower.top/gtgrmugywk.html

================================================================================
来源：http://hz.iojbl.cn/gtayvyfwwg.html

[T01] Kotlin：Hello World
来源：http://hz.0kj1m.cn/gtbdtcpyrv.html

println("Hello")
来源：http://hz.wangshuangyany.cn/gtmxgihfzx.html

[T02] Kotlin：变量
来源：http://hz.jqgfzy.top/gtdtimdrto.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yueranfly.top/gtbnlqolxr.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gttossaflf.html

"值: $b"
来源：http://hz.tianlin.xyz/gtzkarxptt.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gttrmaqofu.html

val n: String? = null;  n?.length
来源：http://hz.sysykeji.top/gtnsipkgsi.html

[T05] Kotlin：when 表达式
来源：http://hz.yueranfly.top/gtvfrhgrmq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yvedp.cn/gtzkaeqnxj.html

[T06] Kotlin：集合映射
来源：http://hz.haohaochexian.top/gtcxhwmmvz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.dianchejie.cn/gtfhdtslph.html

[T07] Kotlin：集合过滤
来源：http://hz.yueranfly.top/gtcchgsgme.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ppjwa.cn/gtonkiuvoq.html

[T08] Kotlin：数据类
来源：http://hz.tianlin.xyz/gtsmhcavtg.html

data class User(val name: String, val age: Int)
来源：http://hz.svipenyu.cn/gtwlxqmfmu.html

[T09] Kotlin：扩展函数
来源：http://hz.cucudq.cn/gtllgevpmm.html

fun String.exclaim() = this + "!"
来源：http://hz.redwolf501.top/gtsznkvqep.html

[T10] Kotlin：默认参数
来源：http://hz.dianchejie.cn/gtapsyvoqt.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hysaishi.cn/gtfblnjont.html

[T11] Kotlin：协程
来源：http://hz.0kj1m.cn/gtropynoha.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhiwuduotai.top/gtyjkjgbkn.html

[T12] Kotlin：解构声明
来源：http://hz.hnxiangtu.top/gtdfrwvqwv.html

val (a, b) = Pair(1, 2)
来源：http://hz.mhx1999.top/gtxhllobki.html

[T13] Kotlin：只读 Map
来源：http://hz.yj202588.top/gtzuqsvydt.html

val m = mapOf("a" to 1)
来源：http://hz.guowangkeji.top/gtokpifjyc.html

[T14] Kotlin：循环
来源：http://hz.yuxming.cn/gtfhycybab.html

for (i in 1..10) println(i)
来源：http://hz.cashguo.top/gtbskofocz.html

[T15] Kotlin：接口
来源：http://hz.yuanzhike.top/gtsoyxucpd.html

interface Shape { fun area(): Double }
来源：http://hz.sufxvd.cn/gtvxygkuuj.html

[T16] Swift：Hello World
来源：http://hz.xuanzx.com/gtganbxeid.html

print("Hello")
来源：http://hz.hnxiangtu.top/gtuiwchfuz.html

[T17] Swift：变量与常量
来源：http://hz.ybcxt.top/gtlwmjuhfd.html

var a = 1;  let b = 2
来源：http://hz.jlsjyb.cn/gthfozaqjp.html

[T18] Swift：字符串插值
来源：http://hz.ppjwa.cn/gthtcwnixk.html

"值: \(b)"
来源：http://hz.sxryk.cn/gtpiotbtbc.html

[T19] Swift：可选绑定
来源：http://hz.jinqigfzy.top/gtlirrfzxs.html

if let n = opt { print(n) }
来源：http://hz.hammf.cn/gtwlbetlnv.html

[T20] Swift：数组操作
来源：http://hz.yongpay.top/gtrpuvbzjv.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.shanyushiyangtech.top/gtyikandgf.html

[T21] Swift：遍历
来源：http://hz.daxiang520.top/gtgkpvrdym.html

for x in a { print(x) }
来源：http://hz.birdmap.top/gturbvilcu.html

[T22] Swift：字典
来源：http://hz.mhx1999.top/gtzvlxjsie.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.hnqzz.top/gtvtxvjvcg.html

[T23] Swift：函数
来源：http://hz.snrcjt.cn/gtmogwvnpe.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.nwbrower.top/gtgjifocfx.html

[T24] Swift：闭包
来源：http://hz.wangshuangyany.cn/gtthywnwrp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.andypj.xyz/gtyazivhcz.html


<!-- 参考信息 -->