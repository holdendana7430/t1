代发 wailian999

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.cheryme.top/gtubpqrtzo.html

[R16] until 等待条件
来源：http://hz.cucudq.cn/gtvssnzzlt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.c1oappe.top/gtmkwnlwop.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtygmekzzs.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.daxiang520.top/gtdvzurhsn.html

[R18] 遍历数组
来源：http://hz.iojbl.cn/gtojagijtx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.shanyushiyangtech.top/gtrcezknut.html

[R19] 数组长度
来源：http://hz.52xcode.cn/gtdtgsrhqc.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtnvidxktp.html

[R20] 关联数组（字典）
来源：http://hz.sysykeji.top/gtagwotwdc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.mhx1999.top/gtjtiwyfok.html

[R21] 字符串长度
来源：http://hz.cucudq.cn/gtlxgbptde.html

echo "${#s}"
来源：http://hz.zhaomingkeji.xyz/gtyussmvys.html

[R22] 截取子串
来源：http://hz.guowangkeji.top/gtsbpbcyyw.html

echo "${s:0:5}"
来源：http://hz.jiagoushi.top/gtylklsiub.html

[R23] 字符串替换
来源：http://hz.iojbl.cn/gtsuyjdzbm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.wangshuangyany.cn/gtzllbihlo.html

[R24] 大小写转换
来源：http://hz.52xcode.cn/gtvpmezbdm.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ydzc1.top/gtjcvcdhjo.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj20258888.top/gtkeoqufjh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hfpthk.cn/gtozstidzh.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtzqpvgwgt.html

now=$(date +%F); echo "$now"
来源：http://hz.jinqigfzy.top/gtjjgcgvap.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gtvdpwotsn.html

echo $((1 + 2 * 3))
来源：http://hz.daria6918.cn/gtjjunfsfw.html

[R28] 浮点运算
来源：http://hz.sysykeji.top/gtzcjzdfrk.html

echo "scale=2; 10/3" | bc
来源：http://hz.jiagoushi.top/gtvrtigqgc.html

[R29] 定义函数
来源：http://hz.feifeiyinyue.top/gtacwtvemp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtxysfbeum.html

[R30] 函数返回状态码
来源：http://hz.hnxiangtu.top/gtlgpuqvgg.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.ivvv.top/gtkhnqmqnk.html

[R31] 局部变量
来源：http://hz.smart0.xyz/gtaswxgrlu.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtthnblxlr.html

[R32] 参数个数校验
来源：http://hz.xuetiantiany.cn/gtoyocpwdj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.snrcjt.cn/gtozvkldkn.html

[R33] 捕获错误并提示行号
来源：http://hz.zdqjudy.top/gtcgtofdvk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ybcxt.top/gtpcelligz.html

[R34] 退出时清理
来源：http://hz.ydzc1.top/gtwwlpvljq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gthealazob.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtloxhwtkf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenzaomai.com/gtwjjwtatr.html

[R36] 并发执行多个任务
来源：http://hz.dianchejie.cn/gtlttnmvzb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.52xcode.cn/gtniqxaqmw.html

[R37] 把输出赋给变量
来源：http://hz.xziqi.cn/gtlvoyiudv.html

files=$(ls -1)
来源：http://hz.yuxming.cn/gtvuumcpkn.html

[R38] 管道串联
来源：http://hz.pengpengdd.cyou/gtgxparsnh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.gotoacloud.top/gtdqlmfzmw.html

[R39] 重定向标准输出与错误
来源：http://hz.shzxlz.cn/gttyjodsrn.html

cmd > out.log 2>&1
来源：http://hz.xziqi.cn/gttezekbts.html

[R40] 追加写日志
来源：http://hz.andypj.xyz/gtcogxughg.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtzybhlylm.html

[R41] 丢弃输出
来源：http://hz.yj20258888.top/gtntnwoiih.html

cmd >/dev/null 2>&1
来源：http://hz.chenlongwang.top/gtzhjizuuz.html

[R42] 输入重定向
来源：http://hz.daxiang520.top/gtttzuzrlx.html

wc -l < a.txt
来源：http://hz.wangdashe.top/gtlwvovdwz.html

[R43] 按名字查找文件
来源：http://hz.fengsongda.top/gtsxtwivlc.html

find . -name "*.log" -type f
来源：http://hz.yanxiufei.cn/gthinsuble.html

[R44] 按修改时间查找
来源：http://hz.cheryme.top/gtbapbdyki.html

find . -mtime -7 -type f
来源：http://hz.ywan-chungtsiang.top/gtbpzltvdy.html

[R45] 批量删除
来源：http://hz.jianghu66.top/gtoeecefta.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtppuobqhr.html

[R46] 递归替换文件内容
来源：http://hz.nwbrower.top/gtmiqkexsh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tian-w.cn/gtqhqezufr.html

[R47] sed 单行替换
来源：http://hz.ydzc1.top/gtvhomrjul.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuxming.cn/gtxjbgrsgx.html

[R48] awk 取指定列
来源：http://hz.snrcjt.cn/gterwbiajd.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinyuanbaomall.cn/gtggqsicjd.html

[R49] awk 带条件
来源：http://hz.fengsongda.top/gtmkauqfgd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtrdvuhauo.html

[R50] awk 求和
来源：http://hz.jyoumei.cn/gtdzicixtb.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ybcxt.top/gttiwcekrm.html

[R51] 排序去重取前几
来源：http://hz.shzxlz.cn/gttiquswad.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hongshengwenyu.top/gtratkxhub.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtidwaixij.html

wc -l a.txt
来源：http://hz.wangshuangyany.cn/gtippmpqsx.html

[R53] 查看文件头与实时尾
来源：http://hz.kuanghao11.cn/gtwplbynyo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtpgwoqenj.html

[R54] 比较两个文件
来源：http://hz.mhx1999.top/gthntsxmdu.html

diff a.txt b.txt
来源：http://hz.zhongyouzk.top/gtsxijacxd.html

[R55] 压缩与解压
来源：http://hz.redwolf501.top/gtnrzdxpgy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jlsjyb.cn/gtwfeexlpj.html

[R56] 远程拷贝
来源：http://hz.guowangkeji.top/gtapusbuyl.html

scp file user@host:/path/
来源：http://hz.cucudq.cn/gtdrruhvuk.html

[R57] 远程执行命令
来源：http://hz.fzhhl.top/gtkgcvsezv.html

ssh user@host 'uptime'
来源：http://hz.c1oappe.top/gtavdytafc.html

[R58] 下载文件
来源：http://hz.xziqi.cn/gtsjskagfq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtamdcpoem.html

[R59] 发 POST JSON
来源：http://hz.ydjk.org.cn/gtkqnsgnfd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.bjfxy.top/gtwtrxwweb.html

[R60] 只看 HTTP 状态码
来源：http://hz.dianchejie.cn/gtfreexntr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtdiwihrlv.html

[R61] 磁盘占用
来源：http://hz.cqqwz.cn/gtoahwsdua.html

df -h;  du -sh *
来源：http://hz.yj20258888.top/gtwrzszcvg.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gtkzifuosd.html

du -ah . | sort -rh | head -10
来源：http://hz.zhixingplan.top/gtlttpelnx.html

[R63] 内存与进程
来源：http://hz.guannengcc.top/gtvcremwov.html

free -h;  ps aux | grep nginx
来源：http://hz.yj20258.top/gtngmynegi.html

[R64] 结束进程
来源：http://hz.sxryk.cn/gttcqmbnvg.html

kill -9 $(pgrep -f app.py)
来源：http://hz.haohaochexian.top/gtjnfrwgze.html

[R65] 查看端口占用
来源：http://hz.hnqzz.top/gtzudojzwy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.xziqi.cn/gtxlsqeaee.html

[R66] 定时任务
来源：http://hz.mhx1999.top/gtklpborlq.html

crontab -e;  crontab -l
来源：http://hz.gotoacloud.top/gtzjrbdqaf.html

[R67] 生成随机十六进制串
来源：http://hz.yvedp.cn/gtqntvqywa.html

openssl rand -hex 16
来源：http://hz.0kj1m.cn/gtbxmhbyvd.html

[R68] 计算文件校验值
来源：http://hz.jinyuanbaomall.cn/gtgrmomnvr.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj20258888.top/gtnpkdogix.html

[R69] 生成随机密码
来源：http://hz.chenjidiqi.icu/gtxewjcpcf.html

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gtigpwdbwy.html

[R70] 时间戳与互转
来源：http://hz.snrcjt.cn/gtkgximovk.html

date +%s;  date -d @1700000000
来源：http://hz.316326.xyz/gtocffclbx.html

[R71] 日期格式化
来源：http://hz.snrcjt.cn/gtanfdocoo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.gotoacloud.top/gthylayaeo.html

[R72] 等待端口就绪
来源：http://hz.svipenyu.cn/gteitwypya.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.snrcjt.cn/gtcyznhctq.html

[R73] 分割大日志
来源：http://hz.hammf.cn/gtlzybsmtc.html

split -l 1000 big.log part_
来源：http://hz.cashguo.top/gticfactcj.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtoepjeryj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.nanxinkj.top/gtrontatkc.html

[R75] 导出环境变量
来源：http://hz.daxiang520.top/gtemthtlfr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtbeectjjn.html

[R76] 使用临时文件
来源：http://hz.ppjwa.cn/gtcpbyynsa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.nanxuanxn.top/gtzrdknxzo.html

[R77] 读取用户输入
来源：http://hz.wangdashe.top/gtyihnqigc.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gtqkchaxqv.html

[R78] 交互式菜单
来源：http://hz.ydzc1.top/gtvpfihzdq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yj20258888.top/gtgrgorkps.html

[R79] 解析命令行选项
来源：http://hz.jqgufenzy.top/gtugapvqen.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.nwbrower.top/gtgunpgyzs.html

[R80] 查看脚本执行耗时
来源：http://hz.shzxlz.cn/gtabkietjt.html

time ./run.sh
来源：http://hz.52xcode.cn/gtpeojqdkf.html

================================================================================
来源：http://hz.tian-w.cn/gtyymwdqgd.html

S. C / C++ 专题
来源：http://hz.daria6918.cn/gtabeaunrr.html

================================================================================
来源：http://hz.xuanzx.com/gtrbzwtuzb.html

[S01] C：Hello World
来源：http://hz.jqgfzy.top/gtobwsmnjs.html

#include <stdio.h>
来源：http://hz.gogol.net.cn/gtrklyrweg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gzhubu.top/gtweeqdnrh.html

[S02] C：变量与格式化输出
来源：http://hz.zhijiandao.cn/gttdgfkdca.html

int a = 10; printf("%d\n", a);
来源：http://hz.ppjwa.cn/gtwfurwyyp.html

[S03] C：读入整数
来源：http://hz.hfpthk.cn/gtuytyauwk.html

int x; scanf("%d", &x);
来源：http://hz.jlsjyb.cn/gtqiiencba.html

[S04] C：字符串复制
来源：http://hz.aibaodan.cn/gtiszdtbow.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.chenlongwang.top/gtbbhblmxk.html

[S05] C：字符串长度
来源：http://hz.snrcjt.cn/gtgosheoei.html

strlen(s)
来源：http://hz.shzxlz.cn/gtmtqnlhck.html

[S06] C：字符串比较
来源：http://hz.cucudq.cn/gtwohysbwy.html

strcmp(a, b) == 0
来源：http://hz.jqgufenzy.top/gtwkmhikgu.html

[S07] C：数组遍历求和
来源：http://hz.havefunace.top/gtqcfycwnl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gtniovdytb.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtpwbrzcax.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.vqdsnc.cn/gtqtzticla.html

[S09] C：结构体定义与初始化
来源：http://hz.jyoumei.cn/gtxmpbubdm.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.cdnleiting.top/gtbwzcdygb.html

[S10] C：指针与解引用
来源：http://hz.nanxinkj.top/gtjxihklkn.html

int *p = &a;  *p = 5;
来源：http://hz.gogol.net.cn/gtkxedfctc.html

[S11] C：逐行读文件
来源：http://hz.ehwqpu.com/gtcwfhcewe.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.guannengcc.top/gtywdxpnoe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.316326.xyz/gtdtrrtgzg.html

fclose(f);
来源：http://hz.redwolf501.top/gtvplltjrp.html

[S12] C：写文件
来源：http://hz.52xcode.cn/gtdaxtotgb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.sweek.top/gtozxzhush.html

[S13] C：宏定义
来源：http://hz.guannengcc.top/gtsswkfwsm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xylfe.cn/gtztaaumml.html

[S14] C：枚举
来源：http://hz.guowangkeji.top/gtezioudhh.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yangfankeji.com/gtcaprosmr.html

[S15] C：类型转换
来源：http://hz.jinqigfzy.top/gtazkehhqa.html

(double) a / b
来源：http://hz.sysykeji.top/gtwkvkmgec.html

[S16] C：位操作置位
来源：http://hz.pycfn.com/gtcftgtigh.html

x |= (1 << 3);
来源：http://hz.zdqjudy.top/gtcgxhojsi.html

[S17] C：安全拼接字符串
来源：http://hz.nanxuanxn.top/gtagfzwqfc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.bjfxy.top/gtwjvbnmat.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtvnvoesdh.html

int main(int argc, char **argv)
来源：http://hz.jinqigufen.top/gtwsjtziwg.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gttwhhegfy.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gttaxjwzxm.html

[S20] C：二分查找
来源：http://hz.hfpthk.cn/gtqqfapisc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jyoumei.cn/gtpeefyfdv.html

[S21] C：字符类别判断
来源：http://hz.aizwys.cn/gthfpubqqc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.wangdashe.top/gtzgfcalxg.html

[S22] C：字符串转数字
来源：http://hz.vqdsnc.cn/gtnlsujrkv.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.gaohongyu789.top/gtastbtzdb.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtpsnqlrrb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.xziqi.cn/gthupkiuyz.html

[S24] C：获取本地时间
来源：http://hz.ydjk.org.cn/gtiypeexaq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shzxlz.cn/gtsndmqcgz.html

[S25] C：内存拷贝
来源：http://hz.cqqwz.cn/gtjjzlfzhp.html

memcpy(dst, src, n);
来源：http://hz.tian-w.cn/gtcyemguts.html

[S26] C：内存清零
来源：http://hz.shanyushiyangtech.top/gtyxnudepy.html

memset(a, 0, sizeof a);
来源：http://hz.tanke756.top/gtamnmivim.html

[S27] C：定义常量
来源：http://hz.shzxlz.cn/gtppfduacg.html

const double PI = 3.14159;
来源：http://hz.xuanzx.com/gtxgestgxq.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtzinstrys.html

static int counter = 0;
来源：http://hz.wangshuangyany.cn/gtpruxuopw.html

[S29] C：变参函数
来源：http://hz.jlsjyb.cn/gtgiagjfhz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yonumen.top/gtjdmawvex.html

[S30] C：头文件保护
来源：http://hz.wangshuangyany.cn/gtotuaneop.html

#ifndef X_H
来源：http://hz.yonumen.top/gtzdkipzif.html

#define X_H
来源：http://hz.aibaodan.cn/gtwbnbsbyl.html

#endif
来源：http://hz.daxiang520.top/gttmqcgfkc.html

[S31] C++：Hello World
来源：http://hz.yueranfly.top/gtnqylytwf.html

#include <iostream>
来源：http://hz.316326.xyz/gtimmfwbxt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.shuidangran.top/gtzezvaypl.html

[S32] C++：字符串
来源：http://hz.dashuyun.cn/gtazjirtkc.html

std::string s = "hi";  s += "!";
来源：http://hz.0kj1m.cn/gtnordfzre.html

[S33] C++：vector 增删
来源：http://hz.hongshengwenyu.top/gtpebyudsk.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gotoacloud.top/gtvpnkuoqz.html

[S34] C++：遍历 vector
来源：http://hz.hfpthk.cn/gtizojycvk.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.jianghu66.top/gtfsjgepgs.html

[S35] C++：map
来源：http://hz.dashuyun.cn/gtomzzfzfg.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.shangyingyoupin.top/gtdyirdyfm.html

[S36] C++：unordered_map
来源：http://hz.yongpay.top/gtipejhdmm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.cqqwz.cn/gtbynveixg.html

[S37] C++：set
来源：http://hz.xinyue.icu/gtntbwopdd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.jqgufenzy.top/gtksiaqohb.html

[S38] C++：排序
来源：http://hz.svipenyu.cn/gttstjvycd.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgufenzy.top/gtwalcndkh.html

[S39] C++：自定义比较器排序
来源：http://hz.hongshengwenyu.top/gtqumipaop.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.yj20258888.top/gtvogeyeth.html

[S40] C++：查找元素
来源：http://hz.zhiwuduotai.top/gtohltabqg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.mhx1999.top/gthsujlubg.html

[S41] C++：类与构造函数
来源：http://hz.hfpthk.cn/gtajiafxxm.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.iojbl.cn/gtcbpikepc.html

[S42] C++：继承与虚函数
来源：http://hz.birdmap.top/gtlbcqdekg.html

class B : public Base { public: void f() override {} };
来源：http://hz.jianghu66.top/gtszxwihkn.html

[S43] C++：智能指针
来源：http://hz.dianchejie.cn/gtgaifbbrx.html

auto p = std::make_unique<int>(5);
来源：http://hz.xuanzx.com/gtcccvjfoo.html

[S44] C++：引用传参
来源：http://hz.zhoulong.xyz/gtlaivieme.html

void inc(int &x) { ++x; }
来源：http://hz.hnqzz.top/gtwfqdingz.html

[S45] C++：lambda
来源：http://hz.cqqwz.cn/gtpznwcosv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.gzhubu.top/gtjnxfdbsq.html

[S46] C++：函数模板
来源：http://hz.aizwys.cn/gtyscbmbjz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigufen.top/gtjuhawcso.html

[S47] C++：结构化绑定遍历
来源：http://hz.pengpengdd.cyou/gtvyftzhiv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ywan-chungtsiang.top/gtfzzcpknu.html

[S48] C++：逐行读文件
来源：http://hz.vqdsnc.cn/gtuhudkufl.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.jianghu66.top/gtvcvevsic.html

while (std::getline(in, line)) { }
来源：http://hz.meibo888.top/gtsohezvqb.html

[S49] C++：写文件
来源：http://hz.jqgufenzy.top/gtrnucmabh.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.c1oappe.top/gtbnlpxexz.html

[S50] C++：格式化数字
来源：http://hz.yonumen.top/gtuatolzdi.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.redwolf501.top/gtkssucpoo.html

[S51] C++：显式类型转换
来源：http://hz.52xcode.cn/gtumaoqaqf.html

static_cast<double>(a) / b
来源：http://hz.bjfxy.top/gtjgrvskxl.html

[S52] C++：const 与 noexcept
来源：http://hz.tianlin.xyz/gtqtvlxxze.html

int size() const noexcept { return n_; }
来源：http://hz.jinqigfzy.top/gteeruysfb.html

[S53] C++：移动语义
来源：http://hz.dashuyun.cn/gtbikunvhg.html

std::vector<int> w = std::move(v);
来源：http://hz.jianghu66.top/gtczfhnqkv.html

[S54] C++：异常处理
来源：http://hz.xuanzx.com/gtybnmpzfz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.c1oappe.top/gtuziwnrzl.html

[S55] C++：结构化绑定
来源：http://hz.birdmap.top/gthtvnyzpe.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.xziqi.cn/gtmvgahoqu.html

[S56] C++：optional
来源：http://hz.9152youxi.cn/gtfhqwrkcd.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.sxryk.cn/gtrpmpjdhc.html

[S57] C++：编译期常量
来源：http://hz.hysaishi.cn/gtvanuujup.html

constexpr int N = 10;
来源：http://hz.xuanzx.com/gtioqanyag.html

[S58] C++：命名空间
来源：http://hz.hammf.cn/gtxmlhnkcx.html

namespace ns { int f() { return 1; } }
来源：http://hz.mhx1999.top/gttzoxtycu.html

[S59] C++：静态断言
来源：http://hz.mhx1999.top/gtnqmwnqix.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.cqqwz.cn/gtghvrsfky.html

[S60] C++：遍历并删除元素
来源：http://hz.nanxinkj.top/gtgrjgynhn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yvedp.cn/gtxotkbqvl.html

================================================================================
来源：http://hz.jqgufenzy.top/gtnkkwnogn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.jinyuanbaomall.cn/gtasjowtyg.html

================================================================================
来源：http://hz.andypj.xyz/gteodgmjyg.html

[T01] Kotlin：Hello World
来源：http://hz.0kj1m.cn/gtvzyxkzkf.html

println("Hello")
来源：http://hz.tanke756.top/gtwmdwgphy.html

[T02] Kotlin：变量
来源：http://hz.fzhhl.top/gtgpbvdbdv.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.redwolf501.top/gtkocbnloa.html

[T03] Kotlin：字符串模板
来源：http://hz.hnxiangtu.top/gtbgirxqjn.html

"值: $b"
来源：http://hz.mhx1999.top/gtkywdwskm.html

[T04] Kotlin：空安全
来源：http://hz.chenjidiqi.icu/gtgiughzbg.html

val n: String? = null;  n?.length
来源：http://hz.hysaishi.cn/gtlddtoiek.html

[T05] Kotlin：when 表达式
来源：http://hz.fzhhl.top/gtqxnxanil.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.jinghuilouyu.cn/gtdvawzjzq.html

[T06] Kotlin：集合映射
来源：http://hz.cheryme.top/gtvfntogtp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yonumen.top/gtsrxxuwri.html

[T07] Kotlin：集合过滤
来源：http://hz.jyoumei.cn/gtykimzlfh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.9152youxi.cn/gtntooepnt.html

[T08] Kotlin：数据类
来源：http://hz.yongpay.top/gtqucpmmro.html

data class User(val name: String, val age: Int)
来源：http://hz.0kj1m.cn/gtwpeunpej.html

[T09] Kotlin：扩展函数
来源：http://hz.fengsongda.top/gtofaqnfht.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtalvpwczf.html

[T10] Kotlin：默认参数
来源：http://hz.jinqigufen.top/gtqxxkmfdr.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hongshengwenyu.top/gtpyeovrus.html

[T11] Kotlin：协程
来源：http://hz.xylfe.cn/gttthmcwpm.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.gotoacloud.top/gtmicbmvnz.html

[T12] Kotlin：解构声明
来源：http://hz.jqgufenzy.top/gtifatycnt.html

val (a, b) = Pair(1, 2)
来源：http://hz.iojbl.cn/gtsycoergj.html

[T13] Kotlin：只读 Map
来源：http://hz.chenzaomai.com/gteefaezpk.html

val m = mapOf("a" to 1)
来源：http://hz.yonumen.top/gtossoygxa.html

[T14] Kotlin：循环
来源：http://hz.cdnleiting.top/gtcypdqirj.html

for (i in 1..10) println(i)
来源：http://hz.redwolf501.top/gtgjvuzcjo.html

[T15] Kotlin：接口
来源：http://hz.yj202588.top/gtahgjrcrj.html

interface Shape { fun area(): Double }
来源：http://hz.daria6918.cn/gtfjqbemcg.html

[T16] Swift：Hello World
来源：http://hz.nanxinkj.top/gtpdmqdzpn.html

print("Hello")
来源：http://hz.shzxlz.cn/gtconcguhh.html

[T17] Swift：变量与常量
来源：http://hz.quarkkingdee.top/gtwonwowox.html

var a = 1;  let b = 2
来源：http://hz.feifeiyinyue.top/gtgncxytlt.html

[T18] Swift：字符串插值
来源：http://hz.xziqi.cn/gtiydgeolr.html

"值: \(b)"
来源：http://hz.yuanzhike.top/gthuhnbeaa.html


<!-- 参考信息 -->