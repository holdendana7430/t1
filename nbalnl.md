代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.xingfuxueyuan.xyz/gtrozmdwlr.html

[R24] 大小写转换
来源：http://hz.vqdsnc.cn/gtfsjnxnea.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gotoacloud.top/gtzwnfipqb.html

[R25] 去后缀 / 去前缀
来源：http://hz.cashguo.top/gtuiwllfkt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.svipenyu.cn/gtrtnwocke.html

[R26] 命令替换
来源：http://hz.wangdashe.top/gteatxuquq.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gtsomykqbu.html

[R27] 算术展开
来源：http://hz.vqdsnc.cn/gtljaanfdr.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtykuesjmb.html

[R28] 浮点运算
来源：http://hz.zhiwuduotai.top/gtriealfrr.html

echo "scale=2; 10/3" | bc
来源：http://hz.nanxuanxn.top/gtkjxzeuis.html

[R29] 定义函数
来源：http://hz.aibaodan.cn/gtrsrirysr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhoulong.xyz/gtyjqpcvwj.html

[R30] 函数返回状态码
来源：http://hz.ybcxt.top/gtvlqqltyj.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhixingplan.top/gtljpdspvf.html

[R31] 局部变量
来源：http://hz.chenlongwang.top/gtrrdmutop.html

f() { local x=1; echo "$x"; }
来源：http://hz.vqdsnc.cn/gttksccgmw.html

[R32] 参数个数校验
来源：http://hz.dashuyun.cn/gtdvmpohfn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxinkj.top/gtrldikdvz.html

[R33] 捕获错误并提示行号
来源：http://hz.birdmap.top/gtshzsozcl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.aizwys.cn/gtohmyvxyv.html

[R34] 退出时清理
来源：http://hz.tianlin.xyz/gtubgkgmxv.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtrchpavcm.html

[R35] 后台执行并等待
来源：http://hz.guannengcc.top/gtrqxdfjaw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ybcxt.top/gtoauaufcj.html

[R36] 并发执行多个任务
来源：http://hz.fzhhl.top/gtbpnqmaim.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.316326.xyz/gtocyvukke.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtoerrugkm.html

files=$(ls -1)
来源：http://hz.jinyuanbaomall.cn/gtpickgyiu.html

[R38] 管道串联
来源：http://hz.c1oappe.top/gtdlrnicih.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tanke756.top/gtgkjptors.html

[R39] 重定向标准输出与错误
来源：http://hz.tanke756.top/gtgpjfeqsi.html

cmd > out.log 2>&1
来源：http://hz.xuetiantiany.cn/gtqajweedd.html

[R40] 追加写日志
来源：http://hz.bjfxy.top/gtvjlnwgkp.html

echo "log" >> out.log
来源：http://hz.jqgufenzy.top/gtqjnirywf.html

[R41] 丢弃输出
来源：http://hz.gaohongyu789.top/gtcdowgziv.html

cmd >/dev/null 2>&1
来源：http://hz.yonumen.top/gtgathzyqo.html

[R42] 输入重定向
来源：http://hz.chenjidiqi.icu/gtiumcdzwm.html

wc -l < a.txt
来源：http://hz.hnqzz.top/gttlxqwcfu.html

[R43] 按名字查找文件
来源：http://hz.chenlongwang.top/gtawksdqvi.html

find . -name "*.log" -type f
来源：http://hz.nanxinkj.top/gtpyhmzdfz.html

[R44] 按修改时间查找
来源：http://hz.hnxiangtu.top/gtfcysksep.html

find . -mtime -7 -type f
来源：http://hz.birdmap.top/gtixzjniuk.html

[R45] 批量删除
来源：http://hz.sysykeji.top/gtbzoxmbpd.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gtpvzhtsjr.html

[R46] 递归替换文件内容
来源：http://hz.xuetiantiany.cn/gtmvjvyoqz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yangfankeji.com/gtnthkhupb.html

[R47] sed 单行替换
来源：http://hz.gzhubu.top/gtmdawaipw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.cheryme.top/gtbefjvzcb.html

[R48] awk 取指定列
来源：http://hz.mhx1999.top/gtlzgwkqqh.html

awk '{print $1, $3}' a.txt
来源：http://hz.kuanghao11.cn/gtvwanctda.html

[R49] awk 带条件
来源：http://hz.aizwys.cn/gtnjyakset.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.snrcjt.cn/gtljvszrpj.html

[R50] awk 求和
来源：http://hz.yj20258888.top/gtyvwcucaw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jiagoushi.top/gteannfdda.html

[R51] 排序去重取前几
来源：http://hz.xziqi.cn/gtmqgxhwso.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtrlkbihzk.html

[R52] 统计行数
来源：http://hz.jinghuilouyu.cn/gtjrwwlkmp.html

wc -l a.txt
来源：http://hz.kuanghao11.cn/gtnrvutomm.html

[R53] 查看文件头与实时尾
来源：http://hz.haohaochexian.top/gtdhgvktxb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sysykeji.top/gtngrxllro.html

[R54] 比较两个文件
来源：http://hz.xuanzx.com/gtyezyoyuy.html

diff a.txt b.txt
来源：http://hz.shangyingyoupin.top/gthtziiwoo.html

[R55] 压缩与解压
来源：http://hz.sufxvd.cn/gtbatlmtzv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.guannengcc.top/gtvxjxhlfr.html

[R56] 远程拷贝
来源：http://hz.cheryme.top/gtwdpjpnva.html

scp file user@host:/path/
来源：http://hz.fengsongda.top/gtmuguhche.html

[R57] 远程执行命令
来源：http://hz.havefunace.top/gtlzyucndq.html

ssh user@host 'uptime'
来源：http://hz.havefunace.top/gtjokthtap.html

[R58] 下载文件
来源：http://hz.xylfe.cn/gtnpnfezue.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.guowangkeji.top/gtvrlcrdly.html

[R59] 发 POST JSON
来源：http://hz.jyoumei.cn/gthheappkk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zycfv.cn/gtmwaokish.html

[R60] 只看 HTTP 状态码
来源：http://hz.gogol.net.cn/gtyxcmqsle.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gzhubu.top/gtdyhadqwm.html

[R61] 磁盘占用
来源：http://hz.cashguo.top/gtcmxiguzu.html

df -h;  du -sh *
来源：http://hz.wangshuangyany.cn/gtwhjkjgfv.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtjetwgqox.html

du -ah . | sort -rh | head -10
来源：http://hz.hnqzz.top/gtfxcgljmq.html

[R63] 内存与进程
来源：http://hz.jinghuilouyu.cn/gtahvlyzll.html

free -h;  ps aux | grep nginx
来源：http://hz.meibo888.top/gtkkorndgt.html

[R64] 结束进程
来源：http://hz.haohaochexian.top/gtbpqavkpw.html

kill -9 $(pgrep -f app.py)
来源：http://hz.52xcode.cn/gtjtkjdmuk.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtfttjiriy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.iojbl.cn/gtmbecxwfe.html

[R66] 定时任务
来源：http://hz.gzhubu.top/gtluvylkyi.html

crontab -e;  crontab -l
来源：http://hz.9152youxi.cn/gtyomqwrmj.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtdjjrbbma.html

openssl rand -hex 16
来源：http://hz.shzxlz.cn/gtbzwlyddz.html

[R68] 计算文件校验值
来源：http://hz.sxryk.cn/gtrdmvoook.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ivvv.top/gtscqequhs.html

[R69] 生成随机密码
来源：http://hz.jqgufenzy.top/gtmlweesgv.html

head -c 16 /dev/urandom | base64
来源：http://hz.xylfe.cn/gthpyhuqnl.html

[R70] 时间戳与互转
来源：http://hz.pengpengdd.cyou/gtmxkaqrtl.html

date +%s;  date -d @1700000000
来源：http://hz.sweek.top/gtbgriieby.html

[R71] 日期格式化
来源：http://hz.dianchejie.cn/gtxjpdovag.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.chenlongwang.top/gtmvuksmbs.html

[R72] 等待端口就绪
来源：http://hz.ybcxt.top/gtjfmvxewv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhiwuduotai.top/gthqiqizai.html

[R73] 分割大日志
来源：http://hz.52xcode.cn/gtyvdbadxy.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtpggunvop.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtfkztplor.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.gogol.net.cn/gtjitwfotf.html

[R75] 导出环境变量
来源：http://hz.shuidangran.top/gtkizrxrac.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtifuinqxt.html

[R76] 使用临时文件
来源：http://hz.hysaishi.cn/gtauhsfvsx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.svipenyu.cn/gtusyikvlp.html

[R77] 读取用户输入
来源：http://hz.jianghu66.top/gtzylawhkc.html

read -rp "请输入: " ans
来源：http://hz.bjfxy.top/gtvwcopoqw.html

[R78] 交互式菜单
来源：http://hz.kuanghao11.cn/gtfcjwlrlr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenzaomai.com/gtmqugxvev.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangkeji.top/gthjurzqpv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yvedp.cn/gtihfejpsv.html

[R80] 查看脚本执行耗时
来源：http://hz.shanyushiyangtech.top/gtoixixbjc.html

time ./run.sh
来源：http://hz.haohaochexian.top/gtigetjkys.html

================================================================================
来源：http://hz.jiagoushi.top/gttzajtiuf.html

S. C / C++ 专题
来源：http://hz.feifeiyinyue.top/gteuvityfj.html

================================================================================
来源：http://hz.jiagoushi.top/gtyzchpkgb.html

[S01] C：Hello World
来源：http://hz.xylfe.cn/gthxwrvjnw.html

#include <stdio.h>
来源：http://hz.aizwys.cn/gtjdoqwpoe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ivvv.top/gtrymenabl.html

[S02] C：变量与格式化输出
来源：http://hz.xylfe.cn/gtqbntnuoa.html

int a = 10; printf("%d\n", a);
来源：http://hz.ivvv.top/gthemfnfpk.html

[S03] C：读入整数
来源：http://hz.shangyingyoupin.top/gtejihatwe.html

int x; scanf("%d", &x);
来源：http://hz.nanxuanxn.top/gtaoqfimjg.html

[S04] C：字符串复制
来源：http://hz.feifeiyinyue.top/gtlryyortc.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhongyouzk.top/gtlfyoisnl.html

[S05] C：字符串长度
来源：http://hz.daxiang520.top/gtrjdebowk.html

strlen(s)
来源：http://hz.jinghuilouyu.cn/gtuxrafuom.html

[S06] C：字符串比较
来源：http://hz.ppjwa.cn/gtksbddnia.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtxfglalut.html

[S07] C：数组遍历求和
来源：http://hz.cashguo.top/gtdipgnlkz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gtltnzuojm.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtlwqhzkui.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hfpthk.cn/gtuzxigsmb.html

[S09] C：结构体定义与初始化
来源：http://hz.sufxvd.cn/gtddxmthkh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.wangshuangyany.cn/gtbrfohcxr.html

[S10] C：指针与解引用
来源：http://hz.jinqigufen.top/gtkeolggtf.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtmukrxwyf.html

[S11] C：逐行读文件
来源：http://hz.guannengcc.top/gtormxfysx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangshuangyany.cn/gtftvwlzbb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.nwbrower.top/gtaxcelfsd.html

fclose(f);
来源：http://hz.9152youxi.cn/gtnqhzrdrd.html

[S12] C：写文件
来源：http://hz.havefunace.top/gtkhvuzppu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yuanzhike.top/gtsbrbqjol.html

[S13] C：宏定义
来源：http://hz.snrcjt.cn/gteroiieao.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtyhrnggqh.html

[S14] C：枚举
来源：http://hz.zycfv.cn/gtbwskwfiq.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.ehwqpu.com/gtezutxxxv.html

[S15] C：类型转换
来源：http://hz.jinqigufen.top/gtkkfdrjxo.html

(double) a / b
来源：http://hz.vqdsnc.cn/gtzqhwbbei.html

[S16] C：位操作置位
来源：http://hz.fengsongda.top/gtwulxcshz.html

x |= (1 << 3);
来源：http://hz.aizwys.cn/gtbuiumrjc.html

[S17] C：安全拼接字符串
来源：http://hz.jinyuanbaomall.cn/gthimhjdej.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.wangdashe.top/gtmewpcxhy.html

[S18] C：命令行参数
来源：http://hz.yangfankeji.com/gtiaovvrjs.html

int main(int argc, char **argv)
来源：http://hz.pycfn.com/gtsnzqmaxv.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtvxsrgezg.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtwbokqwki.html

[S20] C：二分查找
来源：http://hz.hnqzz.top/gtvhwqcocf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gttncvvfgz.html

[S21] C：字符类别判断
来源：http://hz.52xcode.cn/gturuugvxv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.sufxvd.cn/gtikvoccdv.html

[S22] C：字符串转数字
来源：http://hz.hammf.cn/gtyhjwqadn.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.iojbl.cn/gtbjmnynmh.html

[S23] C：随机数
来源：http://hz.ybcxt.top/gtnutdlwin.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jyoumei.cn/gtwqmjogyf.html

[S24] C：获取本地时间
来源：http://hz.yj202588.top/gtweiylupq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hywenlv.cn/gtevxlxwum.html

[S25] C：内存拷贝
来源：http://hz.yueranfly.top/gtnhegptcr.html

memcpy(dst, src, n);
来源：http://hz.shanyushiyangkeji.top/gtfqsnojfd.html

[S26] C：内存清零
来源：http://hz.c1oappe.top/gtcxojfsgp.html

memset(a, 0, sizeof a);
来源：http://hz.yuanzhike.top/gtklmlecbu.html

[S27] C：定义常量
来源：http://hz.sweek.top/gtspycvqqp.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtxvnvhbhc.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtxxxmvpye.html

static int counter = 0;
来源：http://hz.shangyingyoupin.top/gtzdfabhok.html

[S29] C：变参函数
来源：http://hz.havefunace.top/gtdvpixxuj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.c1oappe.top/gtvvqwehcw.html

[S30] C：头文件保护
来源：http://hz.9152youxi.cn/gtbufcwdyk.html

#ifndef X_H
来源：http://hz.ywan-chungtsiang.top/gtuibiyaju.html

#define X_H
来源：http://hz.zhaomingkeji.xyz/gtdfctkyoy.html

#endif
来源：http://hz.zdqjudy.top/gtviamuups.html

[S31] C++：Hello World
来源：http://hz.jqgfzy.top/gtdotmfqem.html

#include <iostream>
来源：http://hz.shanyushiyangtech.top/gtayrsysin.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.zycfv.cn/gtswkaldoe.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtfuerdvfd.html

std::string s = "hi";  s += "!";
来源：http://hz.ydzc1.top/gtlgmkbexw.html

[S33] C++：vector 增删
来源：http://hz.shanyushiyangkeji.top/gtalxiotlz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jiagoushi.top/gtzijbvzcq.html

[S34] C++：遍历 vector
来源：http://hz.hysaishi.cn/gtmybiodkw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xinyue.icu/gtocbkzkdb.html

[S35] C++：map
来源：http://hz.jqgfzy.top/gtxrdcjdll.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.fengsongda.top/gtfgdjrskk.html

[S36] C++：unordered_map
来源：http://hz.iojbl.cn/gtqvmqrfob.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.9152youxi.cn/gtbzhezskh.html

[S37] C++：set
来源：http://hz.xziqi.cn/gtupgdtwyp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.gzhubu.top/gthcrdehfw.html

[S38] C++：排序
来源：http://hz.xinyue.icu/gtlwlmyect.html

std::sort(v.begin(), v.end());
来源：http://hz.kuanghao11.cn/gtjrwjylkd.html

[S39] C++：自定义比较器排序
来源：http://hz.jqgufenzy.top/gthmlywrez.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.fzhhl.top/gtzesikznc.html

[S40] C++：查找元素
来源：http://hz.kuanghao11.cn/gtobofohzx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shanyushiyangkeji.top/gtybkmaizq.html

[S41] C++：类与构造函数
来源：http://hz.jyoumei.cn/gtoiposfwo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.redwolf501.top/gtokkizfwb.html

[S42] C++：继承与虚函数
来源：http://hz.wangshuangyany.cn/gthdagmvgz.html

class B : public Base { public: void f() override {} };
来源：http://hz.daxiang520.top/gtqjzvemdh.html

[S43] C++：智能指针
来源：http://hz.zhongyouzk.top/gtftmcdrtj.html

auto p = std::make_unique<int>(5);
来源：http://hz.vqdsnc.cn/gtiutrdovr.html

[S44] C++：引用传参
来源：http://hz.hongshengwenyu.top/gtissjwxwn.html

void inc(int &x) { ++x; }
来源：http://hz.shzxlz.cn/gtjlpqtejc.html

[S45] C++：lambda
来源：http://hz.chenjidiqi.icu/gtqgcuddtd.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.jinqigufen.top/gtakatpooq.html

[S46] C++：函数模板
来源：http://hz.chenzaomai.com/gtwemfkpgh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.iojbl.cn/gtaprparss.html

[S47] C++：结构化绑定遍历
来源：http://hz.havefunace.top/gtwzufmpni.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.zhijiandao.cn/gtbrvjzmll.html

[S48] C++：逐行读文件
来源：http://hz.c1oappe.top/gtgvdrdupi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.shanyushiyangtech.top/gtgvuxuahn.html

while (std::getline(in, line)) { }
来源：http://hz.jinghuilouyu.cn/gtwnzvvklg.html

[S49] C++：写文件
来源：http://hz.gotoacloud.top/gtkyuxgvil.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.aizwys.cn/gtfyjuqcwe.html

[S50] C++：格式化数字
来源：http://hz.sxryk.cn/gtexjjzumi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yanxiufei.cn/gtzdwpcaea.html

[S51] C++：显式类型转换
来源：http://hz.hnqzz.top/gtxaysizgf.html

static_cast<double>(a) / b
来源：http://hz.quarkkingdee.top/gttqxqcpmz.html

[S52] C++：const 与 noexcept
来源：http://hz.ydzc1.top/gtxykkfdtg.html

int size() const noexcept { return n_; }
来源：http://hz.smart0.xyz/gtewaownnp.html

[S53] C++：移动语义
来源：http://hz.meibo888.top/gtfkdyxgby.html

std::vector<int> w = std::move(v);
来源：http://hz.haohaochexian.top/gtvkssqrnw.html

[S54] C++：异常处理
来源：http://hz.sweek.top/gtsctkchbc.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ywan-chungtsiang.top/gtungssucz.html

[S55] C++：结构化绑定
来源：http://hz.ehwqpu.com/gtnfwhjltl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yongpay.top/gtsmnwufcs.html

[S56] C++：optional
来源：http://hz.sweek.top/gteftxrlou.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.tanke756.top/gtmppoxfuy.html

[S57] C++：编译期常量
来源：http://hz.sweek.top/gtwwviezqj.html

constexpr int N = 10;
来源：http://hz.ydjk.org.cn/gtjiuxmjae.html

[S58] C++：命名空间
来源：http://hz.gogol.net.cn/gtxbtkwexe.html

namespace ns { int f() { return 1; } }
来源：http://hz.yuanzhike.top/gtylvaxnus.html

[S59] C++：静态断言
来源：http://hz.zhijiandao.cn/gtxzkwfdyj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yj20258888.top/gtnejnoewp.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxuanxn.top/gtmcjgriwv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.birdmap.top/gtunkeeuyw.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtegywpnyp.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.sweek.top/gtvffvnloc.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpdurzesy.html

[T01] Kotlin：Hello World
来源：http://hz.jinyuanbaomall.cn/gtcikccfob.html

println("Hello")
来源：http://hz.cdnleiting.top/gtmdtmhlsk.html

[T02] Kotlin：变量
来源：http://hz.zhiwuduotai.top/gtvwxnpviv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gtollglgml.html

[T03] Kotlin：字符串模板
来源：http://hz.jlsjyb.cn/gtuqhizeww.html

"值: $b"
来源：http://hz.shuidangran.top/gtymkmjvxd.html

[T04] Kotlin：空安全
来源：http://hz.xinyue.icu/gtebvzaiob.html

val n: String? = null;  n?.length
来源：http://hz.wangshuangyany.cn/gtsrnnowpr.html

[T05] Kotlin：when 表达式
来源：http://hz.xylfe.cn/gtfpofferc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.smart0.xyz/gtrfdcpnzs.html

[T06] Kotlin：集合映射
来源：http://hz.ppjwa.cn/gtugkpguyd.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hnxiangtu.top/gtkxfabacc.html

[T07] Kotlin：集合过滤
来源：http://hz.mhx1999.top/gtjzwxqdop.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.daria6918.cn/gtxbzsltjz.html

[T08] Kotlin：数据类
来源：http://hz.ehwqpu.com/gtasngymko.html

data class User(val name: String, val age: Int)
来源：http://hz.xziqi.cn/gtxswavckb.html

[T09] Kotlin：扩展函数
来源：http://hz.hammf.cn/gtoyusphuz.html

fun String.exclaim() = this + "!"
来源：http://hz.cqqwz.cn/gtdnzkruwj.html

[T10] Kotlin：默认参数
来源：http://hz.zhoulong.xyz/gtkkajajrf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yanxiufei.cn/gtbyfokqkp.html

[T11] Kotlin：协程
来源：http://hz.hfpthk.cn/gtblxxhyhk.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhaomingkeji.xyz/gtaoxffzoh.html

[T12] Kotlin：解构声明
来源：http://hz.aizwys.cn/gtinauvnox.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtnozyxizw.html

[T13] Kotlin：只读 Map
来源：http://hz.fzhhl.top/gtpmrguzgo.html

val m = mapOf("a" to 1)
来源：http://hz.ywan-chungtsiang.top/gtklcscfdc.html

[T14] Kotlin：循环
来源：http://hz.zhoulong.xyz/gtiyjsvyli.html

for (i in 1..10) println(i)
来源：http://hz.zycfv.cn/gtpvufbxbo.html

[T15] Kotlin：接口
来源：http://hz.yangfankeji.com/gtspgemeho.html

interface Shape { fun area(): Double }
来源：http://hz.ydjk.org.cn/gtpmwteibr.html

[T16] Swift：Hello World
来源：http://hz.shangyingyoupin.top/gtvacbullo.html

print("Hello")
来源：http://hz.yanxiufei.cn/gtzkicbtdp.html

[T17] Swift：变量与常量
来源：http://hz.zdqjudy.top/gtvlvlkaup.html

var a = 1;  let b = 2
来源：http://hz.hysaishi.cn/gtiwkxrdbl.html

[T18] Swift：字符串插值
来源：http://hz.nwbrower.top/gtrebaljbo.html

"值: \(b)"
来源：http://hz.fzhhl.top/gteawpynrb.html

[T19] Swift：可选绑定
来源：http://hz.fzhhl.top/gtnoqjcvsk.html

if let n = opt { print(n) }
来源：http://hz.tian-w.cn/gtugisxdhd.html

[T20] Swift：数组操作
来源：http://hz.pengpengdd.cyou/gtctvkujqd.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.pengpengdd.cyou/gtbtormxtn.html

[T21] Swift：遍历
来源：http://hz.gogol.net.cn/gthpjfbreu.html

for x in a { print(x) }
来源：http://hz.snrcjt.cn/gtzfpgqgck.html

[T22] Swift：字典
来源：http://hz.aizwys.cn/gtxzezmdpz.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.yj20258888.top/gtejyqfdej.html

[T23] Swift：函数
来源：http://hz.guowangkeji.top/gtzcksrlfz.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.hnxiangtu.top/gtaidivvhr.html

[T24] Swift：闭包
来源：http://hz.aizwys.cn/gtttgxdjgo.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.xuanzx.com/gtrbmqzuok.html

[T25] Swift：结构体
来源：http://hz.hammf.cn/gtqpxdrmve.html

struct P { var x: Int }
来源：http://hz.jinghuilouyu.cn/gtkpdejkld.html

[T26] Swift：类与重写
来源：http://hz.jinqigufen.top/gtaclvvpym.html

class A: Base { override func f() {} }
来源：http://hz.shuidangran.top/gtatifpgav.html


<!-- 参考信息 -->