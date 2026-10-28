代发 wailian999

echo "${#arr[@]}"
来源：http://hz.gogol.net.cn/gtlmgwgtct.html

[R20] 关联数组（字典）
来源：http://hz.hysaishi.cn/gtsfqbzvmk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.nanxuanxn.top/gtkgpbzroh.html

[R21] 字符串长度
来源：http://hz.zhijiandao.cn/gtfeeewrbw.html

echo "${#s}"
来源：http://hz.hfpthk.cn/gtydrzcxqp.html

[R22] 截取子串
来源：http://hz.chenjidiqi.icu/gtvlgdajmn.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gtwoajwgdc.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtgdwoquwc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.gaohongyu789.top/gtcehzbnnd.html

[R24] 大小写转换
来源：http://hz.xuetiantiany.cn/gtbajqlddg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ppjwa.cn/gtvgunapik.html

[R25] 去后缀 / 去前缀
来源：http://hz.cheryme.top/gtusoeupyh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dashuyun.cn/gtwufgyhlg.html

[R26] 命令替换
来源：http://hz.haohaochexian.top/gtjbtmibfm.html

now=$(date +%F); echo "$now"
来源：http://hz.zhijiandao.cn/gtnbdjlepk.html

[R27] 算术展开
来源：http://hz.zdqjudy.top/gtwoocqvsj.html

echo $((1 + 2 * 3))
来源：http://hz.jlsjyb.cn/gtjkengakh.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gttfizjfhf.html

echo "scale=2; 10/3" | bc
来源：http://hz.sweek.top/gtatcajiir.html

[R29] 定义函数
来源：http://hz.0kj1m.cn/gtuqnjoejp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hfpthk.cn/gtxwbqvknw.html

[R30] 函数返回状态码
来源：http://hz.xziqi.cn/gtqcsvdgli.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangdashe.top/gtzmiqmeop.html

[R31] 局部变量
来源：http://hz.yueranfly.top/gtsyyjvzof.html

f() { local x=1; echo "$x"; }
来源：http://hz.sufxvd.cn/gtoqydzvhv.html

[R32] 参数个数校验
来源：http://hz.jlsjyb.cn/gtjxinxxle.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258.top/gtkmswvhya.html

[R33] 捕获错误并提示行号
来源：http://hz.zhengqikj.top/gtvhejrxqj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zycfv.cn/gtefwvqrpm.html

[R34] 退出时清理
来源：http://hz.chenlongwang.top/gtwkqwompj.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.ybcxt.top/gtfiqksuut.html

[R35] 后台执行并等待
来源：http://hz.yj202588.top/gtelmfxoso.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hysaishi.cn/gtjuurjcne.html

[R36] 并发执行多个任务
来源：http://hz.zhaomingkeji.xyz/gthgyhtrfw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gtnxzzrkot.html

[R37] 把输出赋给变量
来源：http://hz.yueranfly.top/gtslnflxdk.html

files=$(ls -1)
来源：http://hz.yvedp.cn/gtvvrhtocf.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtnzugcnrb.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hywenlv.cn/gttcpxdxpz.html

[R39] 重定向标准输出与错误
来源：http://hz.nwbrower.top/gtfzyrscqx.html

cmd > out.log 2>&1
来源：http://hz.wangdashe.top/gthjhufyxi.html

[R40] 追加写日志
来源：http://hz.zdqjudy.top/gtfvbkavwg.html

echo "log" >> out.log
来源：http://hz.cheryme.top/gtxdmmnacs.html

[R41] 丢弃输出
来源：http://hz.sysykeji.top/gtfnmwqlyl.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtrfrueire.html

[R42] 输入重定向
来源：http://hz.cashguo.top/gtxfmlrusz.html

wc -l < a.txt
来源：http://hz.xuanzx.com/gtrrdtvuxc.html

[R43] 按名字查找文件
来源：http://hz.shangyingyoupin.top/gtbrwimiwo.html

find . -name "*.log" -type f
来源：http://hz.cqqwz.cn/gtpxkvrtxn.html

[R44] 按修改时间查找
来源：http://hz.ydjk.org.cn/gtcyakvnnr.html

find . -mtime -7 -type f
来源：http://hz.ybcxt.top/gtzkohmzud.html

[R45] 批量删除
来源：http://hz.aizwys.cn/gtqmqrixfg.html

find . -name "*.tmp" -delete
来源：http://hz.cashguo.top/gtydedozjb.html

[R46] 递归替换文件内容
来源：http://hz.9152youxi.cn/gttcinnifg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yj20258.top/gtvxlvnzmq.html

[R47] sed 单行替换
来源：http://hz.jianghu66.top/gtzhfntpsu.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.aibaodan.cn/gtjboczdcf.html

[R48] awk 取指定列
来源：http://hz.gaohongyu789.top/gthjrskmux.html

awk '{print $1, $3}' a.txt
来源：http://hz.guannengcc.top/gtldhedwri.html

[R49] awk 带条件
来源：http://hz.andypj.xyz/gtnaluqfgt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.smart0.xyz/gtskzbykfz.html

[R50] awk 求和
来源：http://hz.nanxuanxn.top/gteijlkknx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.iojbl.cn/gtzkzpblgy.html

[R51] 排序去重取前几
来源：http://hz.havefunace.top/gtnyvjrmsd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.mhx1999.top/gtmtkchzao.html

[R52] 统计行数
来源：http://hz.gogol.net.cn/gttoizetpe.html

wc -l a.txt
来源：http://hz.cucudq.cn/gtkzhdgksf.html

[R53] 查看文件头与实时尾
来源：http://hz.ydjk.org.cn/gtjrbzjccs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.haohaochexian.top/gtifeexkyp.html

[R54] 比较两个文件
来源：http://hz.shzxlz.cn/gtmtcpslfo.html

diff a.txt b.txt
来源：http://hz.shanyushiyangkeji.top/gtongruvff.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gtkhruvrpg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.kuanghao11.cn/gtwhybbyvi.html

[R56] 远程拷贝
来源：http://hz.daxiang520.top/gtliujwjct.html

scp file user@host:/path/
来源：http://hz.nwbrower.top/gtfhwxaers.html

[R57] 远程执行命令
来源：http://hz.shangyingyoupin.top/gtqqwvhjvx.html

ssh user@host 'uptime'
来源：http://hz.cheryme.top/gtsfthuebt.html

[R58] 下载文件
来源：http://hz.yanxiufei.cn/gtlhkeahpt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sufxvd.cn/gtnjvsqqom.html

[R59] 发 POST JSON
来源：http://hz.jlsjyb.cn/gtyoftchnf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.dianchejie.cn/gtdsvqsbcb.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhixingplan.top/gtuohfyhmd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gtmdutrxyi.html

[R61] 磁盘占用
来源：http://hz.tianlin.xyz/gtyqtcgyoj.html

df -h;  du -sh *
来源：http://hz.mhx1999.top/gtepcgmmqv.html

[R62] 找最占空间的文件
来源：http://hz.guowangkeji.top/gtlsyzgbkr.html

du -ah . | sort -rh | head -10
来源：http://hz.ydzc1.top/gtcybiuneh.html

[R63] 内存与进程
来源：http://hz.feifeiyinyue.top/gtpdmndlmm.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangtech.top/gtojqxgkdo.html

[R64] 结束进程
来源：http://hz.cashguo.top/gttkqzqlgr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shzxlz.cn/gtvksovkea.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtisbkdyad.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.zdqjudy.top/gtlgyuwgez.html

[R66] 定时任务
来源：http://hz.shuidangran.top/gtrhcwrkwe.html

crontab -e;  crontab -l
来源：http://hz.yuanzhike.top/gtjqqxmlgh.html

[R67] 生成随机十六进制串
来源：http://hz.wangdashe.top/gtdvhfleqb.html

openssl rand -hex 16
来源：http://hz.pycfn.com/gtejviwvfm.html

[R68] 计算文件校验值
来源：http://hz.sufxvd.cn/gtashbponh.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hnqzz.top/gtvamuwngg.html

[R69] 生成随机密码
来源：http://hz.zhongyouzk.top/gtnmzlgpar.html

head -c 16 /dev/urandom | base64
来源：http://hz.smart0.xyz/gtalfvckeb.html

[R70] 时间戳与互转
来源：http://hz.chenjidiqi.icu/gtmexhljvr.html

date +%s;  date -d @1700000000
来源：http://hz.yueranfly.top/gtrpuoxsza.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtckpebuoc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gogol.net.cn/gtnrvleyer.html

[R72] 等待端口就绪
来源：http://hz.nanxuanxn.top/gtzuvushdr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtyltgoamx.html

[R73] 分割大日志
来源：http://hz.daria6918.cn/gtecitlkco.html

split -l 1000 big.log part_
来源：http://hz.hnqzz.top/gtcwbhzdpy.html

[R74] 批量重命名
来源：http://hz.sysykeji.top/gticmycnnu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.fengsongda.top/gtnmyfieor.html

[R75] 导出环境变量
来源：http://hz.tianlin.xyz/gtxkhphoux.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gthrcrtohk.html

[R76] 使用临时文件
来源：http://hz.guannengcc.top/gtwicsrmhu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gogol.net.cn/gtzabxqyrk.html

[R77] 读取用户输入
来源：http://hz.smart0.xyz/gtfyfhqrqm.html

read -rp "请输入: " ans
来源：http://hz.ivvv.top/gtvpsffkno.html

[R78] 交互式菜单
来源：http://hz.xziqi.cn/gtxxhnggwm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yongpay.top/gtlpsjokrg.html

[R79] 解析命令行选项
来源：http://hz.vqdsnc.cn/gtdmqnhryb.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.quarkkingdee.top/gtvbmlvefy.html

[R80] 查看脚本执行耗时
来源：http://hz.dianchejie.cn/gtsxhxlrob.html

time ./run.sh
来源：http://hz.dianchejie.cn/gtmxnkxzdd.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gteihojofs.html

S. C / C++ 专题
来源：http://hz.sufxvd.cn/gtkloasloo.html

================================================================================
来源：http://hz.fzhhl.top/gtbbkwvjgg.html

[S01] C：Hello World
来源：http://hz.cdnleiting.top/gtbmevrdor.html

#include <stdio.h>
来源：http://hz.cheryme.top/gtdhprxtdl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yangfankeji.com/gtgxtwbgsl.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtsywpltgo.html

int a = 10; printf("%d\n", a);
来源：http://hz.guowangkeji.top/gtnnhmlvfb.html

[S03] C：读入整数
来源：http://hz.zhoulong.xyz/gtimmcakme.html

int x; scanf("%d", &x);
来源：http://hz.zhengqikj.top/gtgeyawhpj.html

[S04] C：字符串复制
来源：http://hz.xziqi.cn/gtwfesbykp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.tanke756.top/gtzvhgxchc.html

[S05] C：字符串长度
来源：http://hz.chenjidiqi.icu/gtyazekvbp.html

strlen(s)
来源：http://hz.hnqzz.top/gtyvkthwqd.html

[S06] C：字符串比较
来源：http://hz.yuanzhike.top/gttddvdpzu.html

strcmp(a, b) == 0
来源：http://hz.chenzaomai.com/gtukakweeb.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtcsjbrotw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hnqzz.top/gtkpmhfvot.html

[S08] C：动态内存分配与释放
来源：http://hz.quarkkingdee.top/gtoilvlbyw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.tian-w.cn/gtonffhqqj.html

[S09] C：结构体定义与初始化
来源：http://hz.snrcjt.cn/gtgklpwkkv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.hongshengwenyu.top/gtphfddtss.html

[S10] C：指针与解引用
来源：http://hz.meibo888.top/gtcrwwipxh.html

int *p = &a;  *p = 5;
来源：http://hz.daria6918.cn/gtkhvlodgc.html

[S11] C：逐行读文件
来源：http://hz.0kj1m.cn/gtqijtowkh.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.dashuyun.cn/gtfapnnpxz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.feifeiyinyue.top/gthrgzkpdn.html

fclose(f);
来源：http://hz.316326.xyz/gtexshpcsl.html

[S12] C：写文件
来源：http://hz.yj202588.top/gtulnkcqnz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.quarkkingdee.top/gtjfgapeqr.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtwrzoxmaq.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnqzz.top/gtwielgnru.html

[S14] C：枚举
来源：http://hz.jlsjyb.cn/gtliajhtzj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.snrcjt.cn/gtgaalplwu.html

[S15] C：类型转换
来源：http://hz.ydjk.org.cn/gtrfkgcliv.html

(double) a / b
来源：http://hz.pengpengdd.cyou/gtxyjqviak.html

[S16] C：位操作置位
来源：http://hz.ppjwa.cn/gtunbwclxk.html

x |= (1 << 3);
来源：http://hz.nanxinkj.top/gtvswqdtjb.html

[S17] C：安全拼接字符串
来源：http://hz.sufxvd.cn/gturjtuzeo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.guannengcc.top/gttfudwevp.html

[S18] C：命令行参数
来源：http://hz.ehwqpu.com/gtwoythhch.html

int main(int argc, char **argv)
来源：http://hz.zycfv.cn/gtomencvzo.html

[S19] C：快速排序
来源：http://hz.hnqzz.top/gtjkdvaxsc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.iojbl.cn/gtdpdrkgmg.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtlmjyxpii.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhoulong.xyz/gtfrcabenh.html

[S21] C：字符类别判断
来源：http://hz.tian-w.cn/gtvbjvkqpa.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shzxlz.cn/gthlzepjwc.html

[S22] C：字符串转数字
来源：http://hz.ywan-chungtsiang.top/gtxepvfbvj.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.kuanghao11.cn/gtoudpbxyj.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtththpikj.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.tian-w.cn/gtpbmrfbyx.html

[S24] C：获取本地时间
来源：http://hz.zhaomingkeji.xyz/gtzkllknsh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nanxuanxn.top/gtmtxaeymm.html

[S25] C：内存拷贝
来源：http://hz.wangshuangyany.cn/gtmxaxmrnw.html

memcpy(dst, src, n);
来源：http://hz.hysaishi.cn/gtocufsebg.html

[S26] C：内存清零
来源：http://hz.xuetiantiany.cn/gtizwhofqj.html

memset(a, 0, sizeof a);
来源：http://hz.meibo888.top/gtzukxtlpf.html

[S27] C：定义常量
来源：http://hz.yonumen.top/gtstnxljlk.html

const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtvpguoogk.html

[S28] C：静态变量
来源：http://hz.zhengqikj.top/gtxadkbhnw.html

static int counter = 0;
来源：http://hz.cdnleiting.top/gtpjqhezcc.html

[S29] C：变参函数
来源：http://hz.shanyushiyangtech.top/gtubaffqyk.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.wangshuangyany.cn/gtiradjayc.html

[S30] C：头文件保护
来源：http://hz.ydjk.org.cn/gteqojmtxj.html

#ifndef X_H
来源：http://hz.iojbl.cn/gtyiithtbr.html

#define X_H
来源：http://hz.cdnleiting.top/gtvcqgxggk.html

#endif
来源：http://hz.ivvv.top/gtnbovlecw.html

[S31] C++：Hello World
来源：http://hz.xylfe.cn/gterohtagj.html

#include <iostream>
来源：http://hz.zhixingplan.top/gthicupbql.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuanzhike.top/gtmzbbaykw.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtykqrtfvy.html

std::string s = "hi";  s += "!";
来源：http://hz.sweek.top/gtiwpodowk.html

[S33] C++：vector 增删
来源：http://hz.nanxuanxn.top/gtbdyabwgk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.fzhhl.top/gtauhlijnd.html

[S34] C++：遍历 vector
来源：http://hz.jinqigfzy.top/gthcvwpybv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daria6918.cn/gtndaliqnp.html

[S35] C++：map
来源：http://hz.jiagoushi.top/gtlgxeaycz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cashguo.top/gteyzeectd.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gthebeakrt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gtgbnleids.html

[S37] C++：set
来源：http://hz.gzhubu.top/gtnvpfcymm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jiagoushi.top/gtxwhdcxos.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtqgakqtyu.html

std::sort(v.begin(), v.end());
来源：http://hz.hnqzz.top/gtdtmampal.html

[S39] C++：自定义比较器排序
来源：http://hz.xziqi.cn/gtuoxirkip.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.vqdsnc.cn/gtsywcogge.html

[S40] C++：查找元素
来源：http://hz.ydzc1.top/gtoiwpetda.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.shzxlz.cn/gtntkqafyd.html

[S41] C++：类与构造函数
来源：http://hz.aizwys.cn/gtftjikawk.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sysykeji.top/gtmvpogfxq.html

[S42] C++：继承与虚函数
来源：http://hz.jianghu66.top/gtygyyzsvg.html

class B : public Base { public: void f() override {} };
来源：http://hz.ydzc1.top/gtxfhhftbd.html

[S43] C++：智能指针
来源：http://hz.hammf.cn/gtxhriyund.html

auto p = std::make_unique<int>(5);
来源：http://hz.jinghuilouyu.cn/gtajqscrup.html

[S44] C++：引用传参
来源：http://hz.hnxiangtu.top/gtyscyrikl.html

void inc(int &x) { ++x; }
来源：http://hz.jlsjyb.cn/gtoqvlzibr.html

[S45] C++：lambda
来源：http://hz.xinyue.icu/gthoqvmdsx.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.hongshengwenyu.top/gtqwyajyyj.html

[S46] C++：函数模板
来源：http://hz.aibaodan.cn/gtcwgcucmy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.xuanzx.com/gthcwpznwr.html

[S47] C++：结构化绑定遍历
来源：http://hz.xingfuxueyuan.xyz/gtprhtvzwb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xylfe.cn/gtpxxvkigf.html

[S48] C++：逐行读文件
来源：http://hz.wangshuangyany.cn/gtnbtqmdat.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gzhubu.top/gtdoghplrj.html

while (std::getline(in, line)) { }
来源：http://hz.xingfuxueyuan.xyz/gtfqalhnji.html

[S49] C++：写文件
来源：http://hz.chenjidiqi.icu/gtplfmnseq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.tian-w.cn/gtifsaslur.html

[S50] C++：格式化数字
来源：http://hz.pengpengdd.cyou/gtevdtehey.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.yuanzhike.top/gtrfrqidnk.html

[S51] C++：显式类型转换
来源：http://hz.sxryk.cn/gtobexdhpx.html

static_cast<double>(a) / b
来源：http://hz.hongshengwenyu.top/gtncjzpyay.html

[S52] C++：const 与 noexcept
来源：http://hz.guannengcc.top/gtjegvhufw.html

int size() const noexcept { return n_; }
来源：http://hz.zhengqikj.top/gtbdugwhep.html

[S53] C++：移动语义
来源：http://hz.ydjk.org.cn/gthlngwxyt.html

std::vector<int> w = std::move(v);
来源：http://hz.jlsjyb.cn/gtuixdhvsh.html

[S54] C++：异常处理
来源：http://hz.daria6918.cn/gtptucyubn.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ivvv.top/gtcpoftaeq.html

[S55] C++：结构化绑定
来源：http://hz.zhongyouzk.top/gtlqxfptgr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.mhx1999.top/gtvtxwovdo.html

[S56] C++：optional
来源：http://hz.redwolf501.top/gtykqesevl.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shangyingyoupin.top/gtaelyrebv.html

[S57] C++：编译期常量
来源：http://hz.yuanzhike.top/gtftoudnsd.html

constexpr int N = 10;
来源：http://hz.xylfe.cn/gthyslvtme.html

[S58] C++：命名空间
来源：http://hz.svipenyu.cn/gtnvewsslt.html

namespace ns { int f() { return 1; } }
来源：http://hz.xylfe.cn/gtdcdahocz.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtronbnlwg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.shuidangran.top/gtnmdztatb.html

[S60] C++：遍历并删除元素
来源：http://hz.aibaodan.cn/gtfsgcdypc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.shanyushiyangtech.top/gtlvpxhnnq.html

================================================================================
来源：http://hz.0kj1m.cn/gtlcheibqf.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.haohaochexian.top/gttflbjuge.html

================================================================================
来源：http://hz.xylfe.cn/gthlnrijvp.html

[T01] Kotlin：Hello World
来源：http://hz.ivvv.top/gtscyqwdzi.html

println("Hello")
来源：http://hz.cucudq.cn/gttsvbkcgn.html

[T02] Kotlin：变量
来源：http://hz.yj20258888.top/gtyzwaaqpf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.9152youxi.cn/gtjmfqbcvm.html

[T03] Kotlin：字符串模板
来源：http://hz.jinqigfzy.top/gtjwhrnnyu.html

"值: $b"
来源：http://hz.zhengqikj.top/gtoilcuedk.html

[T04] Kotlin：空安全
来源：http://hz.cucudq.cn/gtjzkfnsva.html

val n: String? = null;  n?.length
来源：http://hz.zycfv.cn/gtplenwiat.html

[T05] Kotlin：when 表达式
来源：http://hz.guannengcc.top/gtgpwtlszp.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.c1oappe.top/gtmxlncith.html

[T06] Kotlin：集合映射
来源：http://hz.daria6918.cn/gtzsprsdar.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.jqgfzy.top/gtvxqeunky.html

[T07] Kotlin：集合过滤
来源：http://hz.jlsjyb.cn/gtmvefnqmp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.gogol.net.cn/gtbgxkktnx.html

[T08] Kotlin：数据类
来源：http://hz.bjfxy.top/gtythtzraa.html

data class User(val name: String, val age: Int)
来源：http://hz.dianchejie.cn/gtqojgaycq.html

[T09] Kotlin：扩展函数
来源：http://hz.hysaishi.cn/gteesogwro.html

fun String.exclaim() = this + "!"
来源：http://hz.yanxiufei.cn/gtsofldjia.html

[T10] Kotlin：默认参数
来源：http://hz.hnxiangtu.top/gtbvsrzurl.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.yj20258.top/gtjtblmibz.html

[T11] Kotlin：协程
来源：http://hz.fengsongda.top/gthvurrnrd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.zhengqikj.top/gtdjgforcv.html

[T12] Kotlin：解构声明
来源：http://hz.nanxinkj.top/gtdkblqqvd.html

val (a, b) = Pair(1, 2)
来源：http://hz.nwbrower.top/gtdctpligd.html

[T13] Kotlin：只读 Map
来源：http://hz.cdnleiting.top/gtojfupmag.html

val m = mapOf("a" to 1)
来源：http://hz.yj20258.top/gttpsolzxf.html

[T14] Kotlin：循环
来源：http://hz.pycfn.com/gtaaiggxkr.html

for (i in 1..10) println(i)
来源：http://hz.mhx1999.top/gtjdvsgidd.html

[T15] Kotlin：接口
来源：http://hz.chenjidiqi.icu/gtzhunmzdr.html

interface Shape { fun area(): Double }
来源：http://hz.cashguo.top/gtptznplty.html

[T16] Swift：Hello World
来源：http://hz.andypj.xyz/gtefnnlgke.html

print("Hello")
来源：http://hz.hfpthk.cn/gtoezrphrf.html

[T17] Swift：变量与常量
来源：http://hz.c1oappe.top/gtgpiqevvc.html

var a = 1;  let b = 2
来源：http://hz.yj20258888.top/gtapzxvnik.html

[T18] Swift：字符串插值
来源：http://hz.smart0.xyz/gtwgoulmvb.html

"值: \(b)"
来源：http://hz.ehwqpu.com/gtkkhanujf.html

[T19] Swift：可选绑定
来源：http://hz.jinyuanbaomall.cn/gtejbidmpj.html

if let n = opt { print(n) }
来源：http://hz.yonumen.top/gtrjkisczo.html

[T20] Swift：数组操作
来源：http://hz.ydjk.org.cn/gtbsckbmyj.html

var a = [1, 2, 3];  a.append(4)
来源：http://hz.jinqigfzy.top/gtkdyjnrtm.html

[T21] Swift：遍历
来源：http://hz.guannengcc.top/gtvutahhxw.html

for x in a { print(x) }
来源：http://hz.daxiang520.top/gthpzmtxaq.html

[T22] Swift：字典
来源：http://hz.guannengcc.top/gtdgtdzhry.html

var d = ["a": 1];  d["b"] = 2
来源：http://hz.jinghuilouyu.cn/gtvzciwjns.html


<!-- 参考信息 -->