代发 wailian999

echo "${#s}"
来源：http://hz.hfpthk.cn/gtmmwknavm.html

[R22] 截取子串
来源：http://hz.sweek.top/gtplzvdycp.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtbrwwnalm.html

[R23] 字符串替换
来源：http://hz.hywenlv.cn/gtkqucngzc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cashguo.top/gtmkdjidqb.html

[R24] 大小写转换
来源：http://hz.aizwys.cn/gtkfxbwzhp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.pengpengdd.cyou/gtztxxmjwz.html

[R25] 去后缀 / 去前缀
来源：http://hz.svipenyu.cn/gtthpefnzd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.birdmap.top/gtfecwwrlh.html

[R26] 命令替换
来源：http://hz.bjfxy.top/gtjgrhpmjt.html

now=$(date +%F); echo "$now"
来源：http://hz.shangyingyoupin.top/gtnczttwgg.html

[R27] 算术展开
来源：http://hz.snrcjt.cn/gtqpehudgv.html

echo $((1 + 2 * 3))
来源：http://hz.cheryme.top/gtizbbgukv.html

[R28] 浮点运算
来源：http://hz.quarkkingdee.top/gtbevcievr.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhaomingkeji.xyz/gtuoysefmz.html

[R29] 定义函数
来源：http://hz.yuanzhike.top/gtgbqszawp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.zhixingplan.top/gtnyzndnrd.html

[R30] 函数返回状态码
来源：http://hz.jinqigufen.top/gtcrqokzls.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.quarkkingdee.top/gtnyfaofnu.html

[R31] 局部变量
来源：http://hz.yj202588.top/gtdhjcgjux.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtusdayibo.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtwqmvpict.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.andypj.xyz/gtqfqstepz.html

[R33] 捕获错误并提示行号
来源：http://hz.cqqwz.cn/gtutttfnyf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.haohaochexian.top/gtyucncmzo.html

[R34] 退出时清理
来源：http://hz.meibo888.top/gtgxdbqxdq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sufxvd.cn/gtamhqkauo.html

[R35] 后台执行并等待
来源：http://hz.jqgufenzy.top/gtelggrohl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hammf.cn/gtfjaexnhz.html

[R36] 并发执行多个任务
来源：http://hz.yueranfly.top/gtozmewatv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xuanzx.com/gthyuopofh.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gtipxylemk.html

files=$(ls -1)
来源：http://hz.jinqigfzy.top/gtrlgiqqie.html

[R38] 管道串联
来源：http://hz.aizwys.cn/gtzztbwtzy.html

cat a.txt | grep -i error | wc -l
来源：http://hz.haohaochexian.top/gtomcxdyix.html

[R39] 重定向标准输出与错误
来源：http://hz.sxryk.cn/gtwvniowio.html

cmd > out.log 2>&1
来源：http://hz.sysykeji.top/gtohnguwuw.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtanqcpxmx.html

echo "log" >> out.log
来源：http://hz.ybcxt.top/gthosryqfl.html

[R41] 丢弃输出
来源：http://hz.hongshengwenyu.top/gtoewrssxh.html

cmd >/dev/null 2>&1
来源：http://hz.hnqzz.top/gtzpzwhyhj.html

[R42] 输入重定向
来源：http://hz.hongshengwenyu.top/gtcidiaomd.html

wc -l < a.txt
来源：http://hz.zhiwuduotai.top/gtsskadxuu.html

[R43] 按名字查找文件
来源：http://hz.birdmap.top/gtzxzqtyae.html

find . -name "*.log" -type f
来源：http://hz.pengpengdd.cyou/gtgyoiwurm.html

[R44] 按修改时间查找
来源：http://hz.yanxiufei.cn/gtlfvqgdfe.html

find . -mtime -7 -type f
来源：http://hz.hongshengwenyu.top/gtwpadjdpr.html

[R45] 批量删除
来源：http://hz.smart0.xyz/gtcfdsknqk.html

find . -name "*.tmp" -delete
来源：http://hz.guowangkeji.top/gteizomizc.html

[R46] 递归替换文件内容
来源：http://hz.sweek.top/gtcykifeno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.redwolf501.top/gtgwenkcnp.html

[R47] sed 单行替换
来源：http://hz.yj20258.top/gtklkmmpjh.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhongyouzk.top/gtqxkyzozm.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtoinmastp.html

awk '{print $1, $3}' a.txt
来源：http://hz.ybcxt.top/gtbmoiuwsd.html

[R49] awk 带条件
来源：http://hz.wangdashe.top/gtpqehonvp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.52xcode.cn/gtojfxlrje.html

[R50] awk 求和
来源：http://hz.aibaodan.cn/gtotasmpae.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ehwqpu.com/gtedvrqitz.html

[R51] 排序去重取前几
来源：http://hz.tianlin.xyz/gtiurkenlx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.c1oappe.top/gtmlfchfyh.html

[R52] 统计行数
来源：http://hz.shanyushiyangtech.top/gtponlvnva.html

wc -l a.txt
来源：http://hz.jinghuilouyu.cn/gtotovqqsr.html

[R53] 查看文件头与实时尾
来源：http://hz.snrcjt.cn/gtpeqvhidt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.meibo888.top/gthwzhsbys.html

[R54] 比较两个文件
来源：http://hz.xziqi.cn/gtyvkgknmb.html

diff a.txt b.txt
来源：http://hz.shzxlz.cn/gtfgsegmci.html

[R55] 压缩与解压
来源：http://hz.nwbrower.top/gtvroikzbs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhijiandao.cn/gtiffdtiri.html

[R56] 远程拷贝
来源：http://hz.jiagoushi.top/gtwnvdzgvn.html

scp file user@host:/path/
来源：http://hz.c1oappe.top/gtuettftvd.html

[R57] 远程执行命令
来源：http://hz.snrcjt.cn/gtjkhylpbf.html

ssh user@host 'uptime'
来源：http://hz.0kj1m.cn/gtefelwbvq.html

[R58] 下载文件
来源：http://hz.dianchejie.cn/gtkjfwgzsl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinghuilouyu.cn/gtdbthqzks.html

[R59] 发 POST JSON
来源：http://hz.bjfxy.top/gtccynreos.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zhaomingkeji.xyz/gtoiuaqgdu.html

[R60] 只看 HTTP 状态码
来源：http://hz.haohaochexian.top/gtfoqdwcaf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jyoumei.cn/gtwxopbncs.html

[R61] 磁盘占用
来源：http://hz.ivvv.top/gtppobqsdh.html

df -h;  du -sh *
来源：http://hz.yj202588.top/gtwfuigxck.html

[R62] 找最占空间的文件
来源：http://hz.pycfn.com/gtohiihtci.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtjblqlxdd.html

[R63] 内存与进程
来源：http://hz.feifeiyinyue.top/gtemxgnyda.html

free -h;  ps aux | grep nginx
来源：http://hz.hammf.cn/gtrftwvica.html

[R64] 结束进程
来源：http://hz.dianchejie.cn/gtgcwhvpqc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenjidiqi.icu/gttcwruipe.html

[R65] 查看端口占用
来源：http://hz.jqgufenzy.top/gtwyoolonu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.guannengcc.top/gtunophvrv.html

[R66] 定时任务
来源：http://hz.ywan-chungtsiang.top/gtzlhmfzuz.html

crontab -e;  crontab -l
来源：http://hz.yvedp.cn/gtdlrzdjps.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtpmyswwrn.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gtrzflrfty.html

[R68] 计算文件校验值
来源：http://hz.fengsongda.top/gtirlrlvtg.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.nanxinkj.top/gtmnwlypdt.html

[R69] 生成随机密码
来源：http://hz.xylfe.cn/gtcvpsklrg.html

head -c 16 /dev/urandom | base64
来源：http://hz.yj20258.top/gtresgsnuj.html

[R70] 时间戳与互转
来源：http://hz.zhongyouzk.top/gtvcziooqf.html

date +%s;  date -d @1700000000
来源：http://hz.ydzc1.top/gttrmvoffd.html

[R71] 日期格式化
来源：http://hz.redwolf501.top/gtdzslgdys.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.bjfxy.top/gthcuxlbdw.html

[R72] 等待端口就绪
来源：http://hz.ppjwa.cn/gtiewtyhds.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gotoacloud.top/gtlyaqxkkm.html

[R73] 分割大日志
来源：http://hz.daria6918.cn/gtyjhjfwif.html

split -l 1000 big.log part_
来源：http://hz.ivvv.top/gtsizfgocg.html

[R74] 批量重命名
来源：http://hz.ybcxt.top/gtekqjzmqx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zycfv.cn/gtwpvwhcea.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtvgwgjsqo.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtqgzvprfg.html

[R76] 使用临时文件
来源：http://hz.ydzc1.top/gtmdwejdel.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shanyushiyangtech.top/gtpabmkpsq.html

[R77] 读取用户输入
来源：http://hz.yonumen.top/gtatjvmjgz.html

read -rp "请输入: " ans
来源：http://hz.jinqigfzy.top/gtkmbbnvwa.html

[R78] 交互式菜单
来源：http://hz.hnxiangtu.top/gtshhlcwec.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.316326.xyz/gtnnxtsgki.html

[R79] 解析命令行选项
来源：http://hz.hysaishi.cn/gtrxesujlb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fengsongda.top/gtvkjommno.html

[R80] 查看脚本执行耗时
来源：http://hz.yvedp.cn/gtoarmnttg.html

time ./run.sh
来源：http://hz.nanxuanxn.top/gtqrtfqzfm.html

================================================================================
来源：http://hz.haohaochexian.top/gtackljlfw.html

S. C / C++ 专题
来源：http://hz.zhiwuduotai.top/gtkylmujxs.html

================================================================================
来源：http://hz.gotoacloud.top/gtwmzhxvpk.html

[S01] C：Hello World
来源：http://hz.nwbrower.top/gtuqjagzqf.html

#include <stdio.h>
来源：http://hz.redwolf501.top/gtrpyvomwc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yueranfly.top/gtjbffdngf.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtuvbinzzz.html

int a = 10; printf("%d\n", a);
来源：http://hz.iojbl.cn/gtazjcwgjh.html

[S03] C：读入整数
来源：http://hz.jinghuilouyu.cn/gtbyjpeqns.html

int x; scanf("%d", &x);
来源：http://hz.ybcxt.top/gtvfehcjnd.html

[S04] C：字符串复制
来源：http://hz.guowangkeji.top/gtlrqxiugq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.meibo888.top/gtlvuphzhv.html

[S05] C：字符串长度
来源：http://hz.sufxvd.cn/gtywqyjrco.html

strlen(s)
来源：http://hz.cheryme.top/gtrdsyzgvu.html

[S06] C：字符串比较
来源：http://hz.hnxiangtu.top/gtuwzwjagi.html

strcmp(a, b) == 0
来源：http://hz.nwbrower.top/gtxgshiskw.html

[S07] C：数组遍历求和
来源：http://hz.vqdsnc.cn/gtmmwmbzue.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hammf.cn/gtyiydfomx.html

[S08] C：动态内存分配与释放
来源：http://hz.tian-w.cn/gthahapcyi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.hnxiangtu.top/gthqqcqicf.html

[S09] C：结构体定义与初始化
来源：http://hz.chenlongwang.top/gtknkveiny.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sufxvd.cn/gttkeyyayl.html

[S10] C：指针与解引用
来源：http://hz.aibaodan.cn/gtuzqshplp.html

int *p = &a;  *p = 5;
来源：http://hz.hywenlv.cn/gtljlfjvqg.html

[S11] C：逐行读文件
来源：http://hz.sweek.top/gtwkrpvryk.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gttncuulbi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zycfv.cn/gtggbajoil.html

fclose(f);
来源：http://hz.chenzaomai.com/gtoguapmbt.html

[S12] C：写文件
来源：http://hz.xylfe.cn/gtyczbxgmb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zycfv.cn/gtadfwbzql.html

[S13] C：宏定义
来源：http://hz.chenzaomai.com/gtxgpmukcf.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yueranfly.top/gtrqmrrvml.html

[S14] C：枚举
来源：http://hz.52xcode.cn/gtujawjjuh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhiwuduotai.top/gtszharulr.html

[S15] C：类型转换
来源：http://hz.feifeiyinyue.top/gtixxidhyq.html

(double) a / b
来源：http://hz.zhoulong.xyz/gtbtftbyih.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtmxxdizli.html

x |= (1 << 3);
来源：http://hz.daria6918.cn/gtyscjpptb.html

[S17] C：安全拼接字符串
来源：http://hz.yj20258.top/gtbijtnimh.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shanyushiyangkeji.top/gtoerzfadg.html

[S18] C：命令行参数
来源：http://hz.svipenyu.cn/gtihlpdlmo.html

int main(int argc, char **argv)
来源：http://hz.bjfxy.top/gttunabpha.html

[S19] C：快速排序
来源：http://hz.xuetiantiany.cn/gtyhymveev.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtpkgmoian.html

[S20] C：二分查找
来源：http://hz.quarkkingdee.top/gtfebcaofa.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtjzhjxqix.html

[S21] C：字符类别判断
来源：http://hz.guowangkeji.top/gthorqpiqi.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangshuangyany.cn/gtmvtvhxtu.html

[S22] C：字符串转数字
来源：http://hz.cheryme.top/gtcsstuqab.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yanxiufei.cn/gtaecftuay.html

[S23] C：随机数
来源：http://hz.dashuyun.cn/gtnabnlnue.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yonumen.top/gtzynymodo.html

[S24] C：获取本地时间
来源：http://hz.snrcjt.cn/gtfqajrzjv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.daxiang520.top/gtigaxskyz.html

[S25] C：内存拷贝
来源：http://hz.gogol.net.cn/gtvovbdgnr.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gtwakvofpj.html

[S26] C：内存清零
来源：http://hz.ydzc1.top/gtxynbnqws.html

memset(a, 0, sizeof a);
来源：http://hz.zdqjudy.top/gtyyrjylbe.html

[S27] C：定义常量
来源：http://hz.sweek.top/gtzsjylbjo.html

const double PI = 3.14159;
来源：http://hz.sufxvd.cn/gttaoytwzd.html

[S28] C：静态变量
来源：http://hz.aibaodan.cn/gtpnmminhn.html

static int counter = 0;
来源：http://hz.zhongyouzk.top/gtmgybngpd.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtybhpyvyx.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yongpay.top/gtqjbllpdd.html

[S30] C：头文件保护
来源：http://hz.zhijiandao.cn/gtjtglmvce.html

#ifndef X_H
来源：http://hz.316326.xyz/gtjhfzcgqv.html

#define X_H
来源：http://hz.jianghu66.top/gtrlxbkgkb.html

#endif
来源：http://hz.yuanzhike.top/gteyaexeqb.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtkzpangdl.html

#include <iostream>
来源：http://hz.yuxming.cn/gtxyonhqhp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xuetiantiany.cn/gtezbprezr.html

[S32] C++：字符串
来源：http://hz.jqgufenzy.top/gtncilddvn.html

std::string s = "hi";  s += "!";
来源：http://hz.pycfn.com/gtkdwydbox.html

[S33] C++：vector 增删
来源：http://hz.pengpengdd.cyou/gtnmndawuj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.jlsjyb.cn/gthuehtird.html

[S34] C++：遍历 vector
来源：http://hz.ydzc1.top/gtgzytlepw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.havefunace.top/gtaftblouo.html

[S35] C++：map
来源：http://hz.dianchejie.cn/gtsgpbmbob.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj20258888.top/gtocspqsgj.html

[S36] C++：unordered_map
来源：http://hz.yuxming.cn/gtfugaxvne.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sweek.top/gtcyzjnchy.html

[S37] C++：set
来源：http://hz.yj20258.top/gtxzncykxj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.shanyushiyangtech.top/gtjzotxulp.html

[S38] C++：排序
来源：http://hz.jinghuilouyu.cn/gtjxqnkfkd.html

std::sort(v.begin(), v.end());
来源：http://hz.yueranfly.top/gtbepgiyfe.html

[S39] C++：自定义比较器排序
来源：http://hz.sufxvd.cn/gtgdqlzxmr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhiwuduotai.top/gtybqeashh.html

[S40] C++：查找元素
来源：http://hz.nanxinkj.top/gtylzhbmel.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yangfankeji.com/gtwfehyicq.html

[S41] C++：类与构造函数
来源：http://hz.svipenyu.cn/gtfbewzcvr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.tianlin.xyz/gtzqssknfa.html

[S42] C++：继承与虚函数
来源：http://hz.tian-w.cn/gtyblmfdfj.html

class B : public Base { public: void f() override {} };
来源：http://hz.havefunace.top/gtcwmrcsdk.html

[S43] C++：智能指针
来源：http://hz.chenjidiqi.icu/gtmhejzchy.html

auto p = std::make_unique<int>(5);
来源：http://hz.andypj.xyz/gtebhutika.html

[S44] C++：引用传参
来源：http://hz.pycfn.com/gtfqxzhsbh.html

void inc(int &x) { ++x; }
来源：http://hz.cashguo.top/gtcrkhrwlf.html

[S45] C++：lambda
来源：http://hz.nanxinkj.top/gtivsdiryn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhongyouzk.top/gtcmabgfge.html

[S46] C++：函数模板
来源：http://hz.52xcode.cn/gtycchvaeh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhengqikj.top/gtjnlkvjaz.html

[S47] C++：结构化绑定遍历
来源：http://hz.pengpengdd.cyou/gtvytfhosk.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.c1oappe.top/gtfkfwonnp.html

[S48] C++：逐行读文件
来源：http://hz.fengsongda.top/gtsnworhoc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.daxiang520.top/gtefyogttg.html

while (std::getline(in, line)) { }
来源：http://hz.quarkkingdee.top/gtiperbefu.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtfvyhmszy.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.svipenyu.cn/gtqdaqvsig.html

[S50] C++：格式化数字
来源：http://hz.quarkkingdee.top/gticncapkp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zycfv.cn/gtonhdgccc.html

[S51] C++：显式类型转换
来源：http://hz.ybcxt.top/gthbcdyahy.html

static_cast<double>(a) / b
来源：http://hz.wangdashe.top/gtqcajuphy.html

[S52] C++：const 与 noexcept
来源：http://hz.guannengcc.top/gtdgbhxezj.html

int size() const noexcept { return n_; }
来源：http://hz.gogol.net.cn/gtbashxdeo.html

[S53] C++：移动语义
来源：http://hz.zhaomingkeji.xyz/gtlnesrbln.html

std::vector<int> w = std::move(v);
来源：http://hz.xuetiantiany.cn/gtsxzxezwv.html

[S54] C++：异常处理
来源：http://hz.zhiwuduotai.top/gtagzvtgtl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.0kj1m.cn/gtmeyecztz.html

[S55] C++：结构化绑定
来源：http://hz.smart0.xyz/gtvrcmkdsl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.gogol.net.cn/gtknlbgses.html

[S56] C++：optional
来源：http://hz.smart0.xyz/gtmaoyhwmg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.yj20258888.top/gtbmmntble.html

[S57] C++：编译期常量
来源：http://hz.guowangkeji.top/gtjwqlfmej.html

constexpr int N = 10;
来源：http://hz.yuanzhike.top/gtdwgxgbrn.html

[S58] C++：命名空间
来源：http://hz.tianlin.xyz/gtjlvculep.html

namespace ns { int f() { return 1; } }
来源：http://hz.aizwys.cn/gtwbvlqjmu.html

[S59] C++：静态断言
来源：http://hz.jinyuanbaomall.cn/gtgrcybpiv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.gotoacloud.top/gtalhkghip.html

[S60] C++：遍历并删除元素
来源：http://hz.zdqjudy.top/gtmtqxymnw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuxming.cn/gtqjbyrjws.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtixypsnkg.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtzuouwzry.html

================================================================================
来源：http://hz.cheryme.top/gtadnwgzeg.html

[T01] Kotlin：Hello World
来源：http://hz.tianlin.xyz/gtvxlfmera.html

println("Hello")
来源：http://hz.yj20258.top/gtesexydhc.html

[T02] Kotlin：变量
来源：http://hz.cucudq.cn/gtghceitkm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.yongpay.top/gttrdrmdrv.html

[T03] Kotlin：字符串模板
来源：http://hz.0kj1m.cn/gtqprsnnoz.html

"值: $b"
来源：http://hz.sweek.top/gtgtqpzsnf.html

[T04] Kotlin：空安全
来源：http://hz.zhiwuduotai.top/gtquebjval.html

val n: String? = null;  n?.length
来源：http://hz.xuetiantiany.cn/gtucgsfmzw.html

[T05] Kotlin：when 表达式
来源：http://hz.yuxming.cn/gtcodbtrpj.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.chenjidiqi.icu/gtipkyvbty.html

[T06] Kotlin：集合映射
来源：http://hz.shanyushiyangtech.top/gtfcoqwssb.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.haohaochexian.top/gtwgeymtbd.html

[T07] Kotlin：集合过滤
来源：http://hz.aizwys.cn/gtqglahrun.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cheryme.top/gtqcxyesud.html

[T08] Kotlin：数据类
来源：http://hz.cqqwz.cn/gtctpydddl.html

data class User(val name: String, val age: Int)
来源：http://hz.aizwys.cn/gtnmqdsdgb.html

[T09] Kotlin：扩展函数
来源：http://hz.fengsongda.top/gthyxhylse.html

fun String.exclaim() = this + "!"
来源：http://hz.andypj.xyz/gtdlnzczbu.html

[T10] Kotlin：默认参数
来源：http://hz.sxryk.cn/gtfasvsawj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.sufxvd.cn/gtxawetakf.html

[T11] Kotlin：协程
来源：http://hz.smart0.xyz/gtnnjfdmpd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.chenjidiqi.icu/gtoetqjclv.html

[T12] Kotlin：解构声明
来源：http://hz.cucudq.cn/gtnouvyzpb.html

val (a, b) = Pair(1, 2)
来源：http://hz.yuanzhike.top/gtbqkaynhb.html

[T13] Kotlin：只读 Map
来源：http://hz.hongshengwenyu.top/gthrfubegw.html

val m = mapOf("a" to 1)
来源：http://hz.xuetiantiany.cn/gtxnaydfrr.html

[T14] Kotlin：循环
来源：http://hz.jiagoushi.top/gtpiwcldex.html

for (i in 1..10) println(i)
来源：http://hz.kuanghao11.cn/gtgxllrqqy.html

[T15] Kotlin：接口
来源：http://hz.jiagoushi.top/gttggolugy.html

interface Shape { fun area(): Double }
来源：http://hz.yj20258.top/gtaadckcwc.html

[T16] Swift：Hello World
来源：http://hz.chenlongwang.top/gtjwbumlre.html

print("Hello")
来源：http://hz.zhengqikj.top/gtmctpjetd.html

[T17] Swift：变量与常量
来源：http://hz.fzhhl.top/gtclikywlx.html

var a = 1;  let b = 2
来源：http://hz.daria6918.cn/gtfbeulrcp.html

[T18] Swift：字符串插值
来源：http://hz.fengsongda.top/gtsmyyposy.html

"值: \(b)"
来源：http://hz.jiagoushi.top/gtwevlgoug.html

[T19] Swift：可选绑定
来源：http://hz.jyoumei.cn/gtapoqwecy.html

if let n = opt { print(n) }
来源：http://hz.316326.xyz/gtycivdtsb.html

[T20] Swift：数组操作
来源：http://hz.zhixingplan.top/gtxixtyczy.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.tanke756.top/gtipecpotl.html

[T21] Swift：遍历
来源：http://hz.yangfankeji.com/gtahfupibz.html

for x in a { print(x) }
来源：http://hz.jqgfzy.top/gtbctfpjxz.html

[T22] Swift：字典
来源：http://hz.cucudq.cn/gtqefynhfs.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.dashuyun.cn/gtjuzsxndf.html

[T23] Swift：函数
来源：http://hz.hammf.cn/gthvwayxvc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hz.pycfn.com/gtnitlblhm.html

[T24] Swift：闭包
来源：http://hz.dashuyun.cn/gtecwokfcj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://hz.dianchejie.cn/gtnupdhggs.html


<!-- 参考信息 -->