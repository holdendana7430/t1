代发 wailian999

echo "${#arr[@]}"
来源：http://hz.zdqjudy.top/gteieccsjk.html

[R20] 关联数组（字典）
来源：http://hz.dashuyun.cn/gtfmqvppsu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gogol.net.cn/gttjqvppye.html

[R21] 字符串长度
来源：http://hz.cucudq.cn/gtzvstyfle.html

echo "${#s}"
来源：http://hz.yangfankeji.com/gtosiukmaz.html

[R22] 截取子串
来源：http://hz.feifeiyinyue.top/gtdbjrqllv.html

echo "${s:0:5}"
来源：http://hz.aizwys.cn/gtytycqydc.html

[R23] 字符串替换
来源：http://hz.jqgufenzy.top/gtrlngrywu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.sxryk.cn/gtnmwavnap.html

[R24] 大小写转换
来源：http://hz.nwbrower.top/gttmadurlm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cucudq.cn/gtpyssixwh.html

[R25] 去后缀 / 去前缀
来源：http://hz.shanyushiyangtech.top/gtbikshohy.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sweek.top/gtznourlrt.html

[R26] 命令替换
来源：http://hz.cheryme.top/gtuhzplitu.html

now=$(date +%F); echo "$now"
来源：http://hz.sweek.top/gtbfgtqonx.html

[R27] 算术展开
来源：http://hz.zhoulong.xyz/gtxtkdpcxo.html

echo $((1 + 2 * 3))
来源：http://hz.dashuyun.cn/gtcwxngpyv.html

[R28] 浮点运算
来源：http://hz.ppjwa.cn/gtcstivkfn.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuetiantiany.cn/gtoqhhzumi.html

[R29] 定义函数
来源：http://hz.zycfv.cn/gtsqkvhkyx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zycfv.cn/gtwonyiuag.html

[R30] 函数返回状态码
来源：http://hz.cashguo.top/gtphmcqbnd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sweek.top/gtsbieeuvd.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gtborliirj.html

f() { local x=1; echo "$x"; }
来源：http://hz.dashuyun.cn/gtvchumzkr.html

[R32] 参数个数校验
来源：http://hz.jiagoushi.top/gtepultrkc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.tianlin.xyz/gtwljeglym.html

[R33] 捕获错误并提示行号
来源：http://hz.andypj.xyz/gtmowwfyvw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sysykeji.top/gtwrllqsra.html

[R34] 退出时清理
来源：http://hz.yj20258.top/gttebmduoe.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtzdcwxcia.html

[R35] 后台执行并等待
来源：http://hz.yvedp.cn/gtemjixdyv.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gtfgpdkikq.html

[R36] 并发执行多个任务
来源：http://hz.cqqwz.cn/gtqkdfvbbn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shanyushiyangtech.top/gtvevexyew.html

[R37] 把输出赋给变量
来源：http://hz.svipenyu.cn/gtsfyfjdvo.html

files=$(ls -1)
来源：http://hz.meibo888.top/gtjcqjydsn.html

[R38] 管道串联
来源：http://hz.jqgufenzy.top/gtcwcbaesw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.shangyingyoupin.top/gtzraccnec.html

[R39] 重定向标准输出与错误
来源：http://hz.ivvv.top/gtjusnlzts.html

cmd > out.log 2>&1
来源：http://hz.guowangkeji.top/gtwnzdkays.html

[R40] 追加写日志
来源：http://hz.yuxming.cn/gtrqrlghgs.html

echo "log" >> out.log
来源：http://hz.jqgufenzy.top/gtvsbgzpqz.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtvcmwcjmq.html

cmd >/dev/null 2>&1
来源：http://hz.dashuyun.cn/gthhzxblkx.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtfzcqnhfz.html

wc -l < a.txt
来源：http://hz.wangshuangyany.cn/gtmeiqsnti.html

[R43] 按名字查找文件
来源：http://hz.9152youxi.cn/gtdwuvttcm.html

find . -name "*.log" -type f
来源：http://hz.daria6918.cn/gtekeybttj.html

[R44] 按修改时间查找
来源：http://hz.jqgufenzy.top/gthzfxlnvq.html

find . -mtime -7 -type f
来源：http://hz.zhixingplan.top/gtuktwciob.html

[R45] 批量删除
来源：http://hz.jinqigfzy.top/gtkyobjhen.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtgzahltow.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtmdssdsio.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yanxiufei.cn/gtshqgotdr.html

[R47] sed 单行替换
来源：http://hz.hfpthk.cn/gtgkelpppm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhijiandao.cn/gtcqvneath.html

[R48] awk 取指定列
来源：http://hz.yj20258.top/gthtngdyqc.html

awk '{print $1, $3}' a.txt
来源：http://hz.wangdashe.top/gtltptfzcr.html

[R49] awk 带条件
来源：http://hz.guannengcc.top/gtklqygbvv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.chenjidiqi.icu/gtvbrxwuof.html

[R50] awk 求和
来源：http://hz.jianghu66.top/gtlzqcvoyx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.meibo888.top/gtgjnlvvlo.html

[R51] 排序去重取前几
来源：http://hz.pycfn.com/gtkqndzxfu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.andypj.xyz/gtruhkqood.html

[R52] 统计行数
来源：http://hz.sweek.top/gtgowimlsi.html

wc -l a.txt
来源：http://hz.hnqzz.top/gtqzjytqkw.html

[R53] 查看文件头与实时尾
来源：http://hz.jyoumei.cn/gtrypinbwa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aibaodan.cn/gtgdglaodp.html

[R54] 比较两个文件
来源：http://hz.snrcjt.cn/gtkibxhvqu.html

diff a.txt b.txt
来源：http://hz.xuetiantiany.cn/gtazxqyjkq.html

[R55] 压缩与解压
来源：http://hz.jinqigfzy.top/gtonzppmzv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.shanyushiyangtech.top/gtfxcjggju.html

[R56] 远程拷贝
来源：http://hz.mhx1999.top/gtdxqvvwjc.html

scp file user@host:/path/
来源：http://hz.zhoulong.xyz/gtyoxcfxkx.html

[R57] 远程执行命令
来源：http://hz.hammf.cn/gtphspwrzy.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtdsumvhcp.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtuukqzrji.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jqgufenzy.top/gtzigrivxh.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gthuxltpeh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.nwbrower.top/gtyhtrgjmf.html

[R60] 只看 HTTP 状态码
来源：http://hz.gaohongyu789.top/gtodlgjfbk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sweek.top/gtduwvhccf.html

[R61] 磁盘占用
来源：http://hz.yueranfly.top/gtyecoiftb.html

df -h;  du -sh *
来源：http://hz.daria6918.cn/gtjtmnthqz.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gthaeikxzj.html

du -ah . | sort -rh | head -10
来源：http://hz.daria6918.cn/gtpmynqhrj.html

[R63] 内存与进程
来源：http://hz.chenjidiqi.icu/gttkynddug.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtbjkpsuil.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtnjxjjymh.html

kill -9 $(pgrep -f app.py)
来源：http://hz.zdqjudy.top/gtzgpwyeon.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtautemxjk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zhengqikj.top/gtznspnigx.html

[R66] 定时任务
来源：http://hz.chenzaomai.com/gtsyistpun.html

crontab -e;  crontab -l
来源：http://hz.iojbl.cn/gtvnovayry.html

[R67] 生成随机十六进制串
来源：http://hz.0kj1m.cn/gtzilkybho.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gtwjldmhpe.html

[R68] 计算文件校验值
来源：http://hz.hywenlv.cn/gtiljrtogx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.jlsjyb.cn/gtlgnmijba.html

[R69] 生成随机密码
来源：http://hz.tian-w.cn/gtxjtiqspb.html

head -c 16 /dev/urandom | base64
来源：http://hz.jiagoushi.top/gtdomlpfjf.html

[R70] 时间戳与互转
来源：http://hz.ybcxt.top/gtrifmcjzb.html

date +%s;  date -d @1700000000
来源：http://hz.guowangkeji.top/gtusyzbfko.html

[R71] 日期格式化
来源：http://hz.fengsongda.top/gtolpgpmbw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.0kj1m.cn/gtrdhsxdwp.html

[R72] 等待端口就绪
来源：http://hz.jinghuilouyu.cn/gtdapfeotb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cashguo.top/gtxxadmvbp.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtxpcjondo.html

split -l 1000 big.log part_
来源：http://hz.wangdashe.top/gtrzsddtkl.html

[R74] 批量重命名
来源：http://hz.ppjwa.cn/gtecoafxcp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jyoumei.cn/gtnyrakghv.html

[R75] 导出环境变量
来源：http://hz.gzhubu.top/gtiedlbqwa.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cucudq.cn/gteofnhmux.html

[R76] 使用临时文件
来源：http://hz.yueranfly.top/gtypdlaint.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shzxlz.cn/gtjcnhunnq.html

[R77] 读取用户输入
来源：http://hz.52xcode.cn/gtmlqwqyqt.html

read -rp "请输入: " ans
来源：http://hz.nanxuanxn.top/gtobfzssis.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtryvtgosu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.aibaodan.cn/gtunnorrsz.html

[R79] 解析命令行选项
来源：http://hz.c1oappe.top/gtckixwnni.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.tian-w.cn/gtccmvtzzj.html

[R80] 查看脚本执行耗时
来源：http://hz.sxryk.cn/gtbnwcyvvf.html

time ./run.sh
来源：http://hz.chenzaomai.com/gtjuhhkllc.html

================================================================================
来源：http://hz.pycfn.com/gttuhleozt.html

S. C / C++ 专题
来源：http://hz.c1oappe.top/gtkxjctuvr.html

================================================================================
来源：http://hz.andypj.xyz/gtaipzbpzg.html

[S01] C：Hello World
来源：http://hz.ybcxt.top/gtlmqyxwfj.html

#include <stdio.h>
来源：http://hz.yuxming.cn/gtjaatmkmx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jlsjyb.cn/gtdjmonnkl.html

[S02] C：变量与格式化输出
来源：http://hz.chenjidiqi.icu/gtoggbfflq.html

int a = 10; printf("%d\n", a);
来源：http://hz.chenzaomai.com/gtqnzyarkw.html

[S03] C：读入整数
来源：http://hz.sxryk.cn/gtjmusgwbh.html

int x; scanf("%d", &x);
来源：http://hz.fzhhl.top/gtvhywigog.html

[S04] C：字符串复制
来源：http://hz.gzhubu.top/gtkjpjroja.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.daxiang520.top/gttdvnszoa.html

[S05] C：字符串长度
来源：http://hz.yueranfly.top/gtgsawdegi.html

strlen(s)
来源：http://hz.tianlin.xyz/gtdzrfwemn.html

[S06] C：字符串比较
来源：http://hz.cashguo.top/gtkgacmgsv.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtfdhvgdtb.html

[S07] C：数组遍历求和
来源：http://hz.wangdashe.top/gtxikqvcrs.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yangfankeji.com/gtekvadceh.html

[S08] C：动态内存分配与释放
来源：http://hz.zdqjudy.top/gtbfgmgjve.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj20258.top/gticxnesen.html

[S09] C：结构体定义与初始化
来源：http://hz.fzhhl.top/gtrlpztqpb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yj202588.top/gtdokmogoz.html

[S10] C：指针与解引用
来源：http://hz.tanke756.top/gtfhgiuxbi.html

int *p = &a;  *p = 5;
来源：http://hz.tianlin.xyz/gtiyalehxk.html

[S11] C：逐行读文件
来源：http://hz.hnqzz.top/gtqrxqiyhr.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cashguo.top/gtttvigatb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yvedp.cn/gteesmwsxq.html

fclose(f);
来源：http://hz.shangyingyoupin.top/gtqcdqegrq.html

[S12] C：写文件
来源：http://hz.cdnleiting.top/gtgmkpkfsy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.9152youxi.cn/gthqpmsawf.html

[S13] C：宏定义
来源：http://hz.sweek.top/gtesvhpwvr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.iojbl.cn/gtvhoobisf.html

[S14] C：枚举
来源：http://hz.hnqzz.top/gthxagsvdm.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.chenlongwang.top/gtajkmihsy.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gteajzzctm.html

(double) a / b
来源：http://hz.bjfxy.top/gtlofhbnxa.html

[S16] C：位操作置位
来源：http://hz.andypj.xyz/gtfsmqszgh.html

x |= (1 << 3);
来源：http://hz.ywan-chungtsiang.top/gtjmbrluks.html

[S17] C：安全拼接字符串
来源：http://hz.svipenyu.cn/gtgumvidvr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ybcxt.top/gtzfdbrxvh.html

[S18] C：命令行参数
来源：http://hz.nanxinkj.top/gtmaejpgcj.html

int main(int argc, char **argv)
来源：http://hz.yj20258.top/gtmndaaori.html

[S19] C：快速排序
来源：http://hz.shzxlz.cn/gtnqlaqdtz.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtvemlduqn.html

[S20] C：二分查找
来源：http://hz.hywenlv.cn/gtswsdibgz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhengqikj.top/gtvexefvxp.html

[S21] C：字符类别判断
来源：http://hz.daria6918.cn/gtxccvyjiw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xuetiantiany.cn/gthacbcxno.html

[S22] C：字符串转数字
来源：http://hz.shanyushiyangtech.top/gtawzgkdfm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cdnleiting.top/gtfmhzyxwx.html

[S23] C：随机数
来源：http://hz.xingfuxueyuan.xyz/gtdjdffeox.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.bjfxy.top/gtxkguywcf.html

[S24] C：获取本地时间
来源：http://hz.daxiang520.top/gtimyrdpko.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtjddfidyk.html

[S25] C：内存拷贝
来源：http://hz.sysykeji.top/gtmxxbidce.html

memcpy(dst, src, n);
来源：http://hz.daxiang520.top/gtnjzckccl.html

[S26] C：内存清零
来源：http://hz.shangyingyoupin.top/gtastrizyy.html

memset(a, 0, sizeof a);
来源：http://hz.dianchejie.cn/gtrdxgevov.html

[S27] C：定义常量
来源：http://hz.mhx1999.top/gtlzptakoe.html

const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gttlzhlovy.html

[S28] C：静态变量
来源：http://hz.zdqjudy.top/gtdulgypfy.html

static int counter = 0;
来源：http://hz.daria6918.cn/gtyaxpgzct.html

[S29] C：变参函数
来源：http://hz.jinqigfzy.top/gtopqidtxy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.cqqwz.cn/gtfsfhapca.html

[S30] C：头文件保护
来源：http://hz.pengpengdd.cyou/gtnxzecljk.html

#ifndef X_H
来源：http://hz.hongshengwenyu.top/gtwlvblznc.html

#define X_H
来源：http://hz.gzhubu.top/gtuohcebca.html

#endif
来源：http://hz.zhaomingkeji.xyz/gthvtqlmsm.html

[S31] C++：Hello World
来源：http://hz.hfpthk.cn/gtjojuicht.html

#include <iostream>
来源：http://hz.fzhhl.top/gtvziwtddf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ppjwa.cn/gtvipllgen.html

[S32] C++：字符串
来源：http://hz.snrcjt.cn/gtdcdzhecp.html

std::string s = "hi";  s += "!";
来源：http://hz.zhoulong.xyz/gtflgvkrur.html

[S33] C++：vector 增删
来源：http://hz.zdqjudy.top/gtdxdzrxsw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.ybcxt.top/gtsixoharq.html

[S34] C++：遍历 vector
来源：http://hz.andypj.xyz/gthkzubtqa.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.0kj1m.cn/gtvkkyhcud.html

[S35] C++：map
来源：http://hz.xylfe.cn/gtjhcyhaza.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zdqjudy.top/gtypjgnffc.html

[S36] C++：unordered_map
来源：http://hz.jianghu66.top/gtrpwjybnz.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtnmusvnzj.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtzhbzsxqb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ehwqpu.com/gtutwgsnro.html

[S38] C++：排序
来源：http://hz.hammf.cn/gtjcxxjuql.html

std::sort(v.begin(), v.end());
来源：http://hz.aizwys.cn/gtpukethff.html

[S39] C++：自定义比较器排序
来源：http://hz.hnqzz.top/gthsixcxnq.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.aibaodan.cn/gtodyskcjs.html

[S40] C++：查找元素
来源：http://hz.hnqzz.top/gtmftkqiws.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yvedp.cn/gtoebbckeg.html

[S41] C++：类与构造函数
来源：http://hz.snrcjt.cn/gtbtsupjdc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.chenzaomai.com/gtyuubjfom.html

[S42] C++：继承与虚函数
来源：http://hz.zdqjudy.top/gtceyweqjz.html

class B : public Base { public: void f() override {} };
来源：http://hz.wangdashe.top/gtjioziqzx.html

[S43] C++：智能指针
来源：http://hz.tanke756.top/gtykswopwd.html

auto p = std::make_unique<int>(5);
来源：http://hz.smart0.xyz/gtwphkuakj.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtoytlbxws.html

void inc(int &x) { ++x; }
来源：http://hz.zycfv.cn/gtqbcespxz.html

[S45] C++：lambda
来源：http://hz.shangyingyoupin.top/gtgolaievx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.bjfxy.top/gtfxcnngiv.html

[S46] C++：函数模板
来源：http://hz.nanxuanxn.top/gtcizfynwu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sxryk.cn/gtpbjafluo.html

[S47] C++：结构化绑定遍历
来源：http://hz.ybcxt.top/gtozpxtkrs.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ivvv.top/gtrcyhroof.html

[S48] C++：逐行读文件
来源：http://hz.zhixingplan.top/gtbjcsgxpv.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hysaishi.cn/gtcbwuhzwo.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtydohdjem.html

[S49] C++：写文件
来源：http://hz.52xcode.cn/gtlpekrgub.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yuxming.cn/gtsgjygaep.html

[S50] C++：格式化数字
来源：http://hz.52xcode.cn/gtomttmqqk.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.sufxvd.cn/gtcmkhefbg.html

[S51] C++：显式类型转换
来源：http://hz.hongshengwenyu.top/gtpqxpqzad.html

static_cast<double>(a) / b
来源：http://hz.9152youxi.cn/gtwfbjkbux.html

[S52] C++：const 与 noexcept
来源：http://hz.zhongyouzk.top/gtzsthysfc.html

int size() const noexcept { return n_; }
来源：http://hz.daxiang520.top/gtznqzgbsv.html

[S53] C++：移动语义
来源：http://hz.xinyue.icu/gtgvkfvikk.html

std::vector<int> w = std::move(v);
来源：http://hz.birdmap.top/gtsinlviiw.html

[S54] C++：异常处理
来源：http://hz.shanyushiyangkeji.top/gtsvmbixhv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.nanxinkj.top/gtibndcuzx.html

[S55] C++：结构化绑定
来源：http://hz.zhaomingkeji.xyz/gtigvwacoj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhixingplan.top/gtfkopjshx.html

[S56] C++：optional
来源：http://hz.zhijiandao.cn/gtcgmslwqh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj202588.top/gttuytawyi.html

[S57] C++：编译期常量
来源：http://hz.shzxlz.cn/gtqrlojgci.html

constexpr int N = 10;
来源：http://hz.snrcjt.cn/gtdlazaiqy.html

[S58] C++：命名空间
来源：http://hz.c1oappe.top/gtsfmhjryd.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangtech.top/gteqkmxods.html

[S59] C++：静态断言
来源：http://hz.xuanzx.com/gtbdbnowdy.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jyoumei.cn/gtxxqogdhz.html

[S60] C++：遍历并删除元素
来源：http://hz.daria6918.cn/gtputwimbp.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.xinyue.icu/gtpkzwfxbe.html

================================================================================
来源：http://hz.meibo888.top/gtahvmrjpe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.meibo888.top/gtiduyjyim.html

================================================================================
来源：http://hz.kuanghao11.cn/gtlufqvfwe.html

[T01] Kotlin：Hello World
来源：http://hz.tanke756.top/gtmyjwomln.html

println("Hello")
来源：http://hz.ydzc1.top/gtrsetbvze.html

[T02] Kotlin：变量
来源：http://hz.hfpthk.cn/gttftrwpmv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.sweek.top/gtobozdvvk.html

[T03] Kotlin：字符串模板
来源：http://hz.pycfn.com/gtavunrduf.html

"值: $b"
来源：http://hz.redwolf501.top/gtjvburazu.html

[T04] Kotlin：空安全
来源：http://hz.zycfv.cn/gtuwskjttt.html

val n: String? = null;  n?.length
来源：http://hz.chenzaomai.com/gtgwbpwulc.html

[T05] Kotlin：when 表达式
来源：http://hz.yonumen.top/gtsheyzfgm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hfpthk.cn/gtkjxvckez.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtxennyenm.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cheryme.top/gtychtazwz.html

[T07] Kotlin：集合过滤
来源：http://hz.tian-w.cn/gtwaijzwsh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yueranfly.top/gtlyfyiyku.html

[T08] Kotlin：数据类
来源：http://hz.zhijiandao.cn/gtzrgixxjo.html

data class User(val name: String, val age: Int)
来源：http://hz.ehwqpu.com/gtvjjrmbhh.html

[T09] Kotlin：扩展函数
来源：http://hz.yvedp.cn/gtwdihrfpa.html

fun String.exclaim() = this + "!"
来源：http://hz.bjfxy.top/gtwotocesy.html

[T10] Kotlin：默认参数
来源：http://hz.hammf.cn/gtdfrpvpix.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.ybcxt.top/gtfcyghrns.html

[T11] Kotlin：协程
来源：http://hz.xinyue.icu/gtnxpvwsei.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.dianchejie.cn/gtbrojhjtv.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtwwibdtar.html

val (a, b) = Pair(1, 2)
来源：http://hz.svipenyu.cn/gtfltiyxee.html

[T13] Kotlin：只读 Map
来源：http://hz.nwbrower.top/gticgwdolz.html

val m = mapOf("a" to 1)
来源：http://hz.jianghu66.top/gtsrzpbzfw.html

[T14] Kotlin：循环
来源：http://hz.havefunace.top/gtzsglbude.html

for (i in 1..10) println(i)
来源：http://hz.jqgfzy.top/gtghywmwju.html

[T15] Kotlin：接口
来源：http://hz.pengpengdd.cyou/gthopebqwa.html

interface Shape { fun area(): Double }
来源：http://hz.jinqigfzy.top/gtjgeopixv.html

[T16] Swift：Hello World
来源：http://hz.jinyuanbaomall.cn/gtxiyleeel.html

print("Hello")
来源：http://hz.yvedp.cn/gtixspdmle.html

[T17] Swift：变量与常量
来源：http://hz.52xcode.cn/gtyuveoxym.html

var a = 1;  let b = 2
来源：http://hz.jqgufenzy.top/gtazlpjuxm.html

[T18] Swift：字符串插值
来源：http://hz.kuanghao11.cn/gtzsutlrvv.html

"值: \(b)"
来源：http://hz.ivvv.top/gtwlrdhbch.html

[T19] Swift：可选绑定
来源：http://hz.feifeiyinyue.top/gtehaakpho.html

if let n = opt { print(n) }
来源：http://hz.zhijiandao.cn/gtanemzhiu.html

[T20] Swift：数组操作
来源：http://hz.snrcjt.cn/gtwaecjsuc.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.dashuyun.cn/gtfroyosny.html

[T21] Swift：遍历
来源：http://hz.wangdashe.top/gtdxgxsgpm.html

for x in a { print(x) }
来源：http://hz.zhoulong.xyz/gtxlkwtiyl.html

[T22] Swift：字典
来源：http://hz.smart0.xyz/gtaojqdzyg.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.52xcode.cn/gtqbxflull.html


<!-- 参考信息 -->