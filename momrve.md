代发 wailian999

case "$1" in
来源：http://hz.xinyue.icu/gtlzgvipad.html

start) echo "启动" ;;
来源：http://hz.cucudq.cn/gtlrpsthkx.html

stop)  echo "停止" ;;
来源：http://hz.jiagoushi.top/gtcmoadott.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtyxlgnbgo.html

esac
来源：http://hz.guowangkeji.top/gtxiyjyarg.html

[R12] for 遍历文件
来源：http://hz.ydjk.org.cn/gtlukxflep.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hongshengwenyu.top/gtegxjaecb.html

[R13] for 计数循环
来源：http://hz.ivvv.top/gtmcxcpitv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhijiandao.cn/gtjskmxzau.html

[R14] C 风格 for
来源：http://hz.zhengqikj.top/gtrwwoylhq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jlsjyb.cn/gtkdezzery.html

[R15] while 逐行读文件
来源：http://hz.ehwqpu.com/gtqxviqciu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.haohaochexian.top/gttvybnnrw.html

[R16] until 等待条件
来源：http://hz.bjfxy.top/gtvhnsldei.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.pycfn.com/gtitztcxsl.html

[R17] 数组定义与取值
来源：http://hz.jyoumei.cn/gtsenzrlyx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.gzhubu.top/gtkhwhdpus.html

[R18] 遍历数组
来源：http://hz.hammf.cn/gttonjarzz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.jqgfzy.top/gtgoimwwzl.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtmmdaifle.html

echo "${#arr[@]}"
来源：http://hz.zhongyouzk.top/gtrpldykuj.html

[R20] 关联数组（字典）
来源：http://hz.bjfxy.top/gttkclzeob.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hysaishi.cn/gtsyqftrnl.html

[R21] 字符串长度
来源：http://hz.feifeiyinyue.top/gtolckwbat.html

echo "${#s}"
来源：http://hz.sxryk.cn/gtnlhufkan.html

[R22] 截取子串
来源：http://hz.zhengqikj.top/gtuwavzueo.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtkfdrqwed.html

[R23] 字符串替换
来源：http://hz.dashuyun.cn/gtanlmjixd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yuanzhike.top/gtisutlhuz.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtcvojcrnf.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ehwqpu.com/gtgsivlwbc.html

[R25] 去后缀 / 去前缀
来源：http://hz.sysykeji.top/gtyhkclbqx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hywenlv.cn/gtdolrdsrj.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gtouqqcmqa.html

now=$(date +%F); echo "$now"
来源：http://hz.zhaomingkeji.xyz/gtuqwttvpz.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gtxqugyply.html

echo $((1 + 2 * 3))
来源：http://hz.yangfankeji.com/gtdqwopqmp.html

[R28] 浮点运算
来源：http://hz.hongshengwenyu.top/gtjcuqjbox.html

echo "scale=2; 10/3" | bc
来源：http://hz.ivvv.top/gtacinuklf.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gtwxqpiwfz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.0kj1m.cn/gtpjwdhhhi.html

[R30] 函数返回状态码
来源：http://hz.xuanzx.com/gtahvgcasv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.9152youxi.cn/gtqwozybhj.html

[R31] 局部变量
来源：http://hz.xziqi.cn/gtokcifuxk.html

f() { local x=1; echo "$x"; }
来源：http://hz.hnqzz.top/gtuvtovixy.html

[R32] 参数个数校验
来源：http://hz.yuxming.cn/gtuxxaecdh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ybcxt.top/gtknihisqb.html

[R33] 捕获错误并提示行号
来源：http://hz.0kj1m.cn/gtrwywwvsi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.chenjidiqi.icu/gtpyjzmqjh.html

[R34] 退出时清理
来源：http://hz.52xcode.cn/gttdayxdvn.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.nwbrower.top/gtprmbfsjc.html

[R35] 后台执行并等待
来源：http://hz.andypj.xyz/gtlxocyxwz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.52xcode.cn/gtjqthzvud.html

[R36] 并发执行多个任务
来源：http://hz.hfpthk.cn/gtfszmaipj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.bjfxy.top/gtosfmpqjq.html

[R37] 把输出赋给变量
来源：http://hz.gotoacloud.top/gtfajhuyjr.html

files=$(ls -1)
来源：http://hz.tanke756.top/gtcesaviim.html

[R38] 管道串联
来源：http://hz.hammf.cn/gtptdwqswv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtmdhqxcox.html

[R39] 重定向标准输出与错误
来源：http://hz.tanke756.top/gtlbgnsbjt.html

cmd > out.log 2>&1
来源：http://hz.hongshengwenyu.top/gtrpizjffx.html

[R40] 追加写日志
来源：http://hz.yuanzhike.top/gtbqrqgjjn.html

echo "log" >> out.log
来源：http://hz.iojbl.cn/gthluzxyel.html

[R41] 丢弃输出
来源：http://hz.dashuyun.cn/gtbaftlkab.html

cmd >/dev/null 2>&1
来源：http://hz.c1oappe.top/gtkkjngoux.html

[R42] 输入重定向
来源：http://hz.shzxlz.cn/gtiggbsxec.html

wc -l < a.txt
来源：http://hz.fengsongda.top/gtekyqwjnk.html

[R43] 按名字查找文件
来源：http://hz.gzhubu.top/gtmqmmpona.html

find . -name "*.log" -type f
来源：http://hz.sweek.top/gtkgnrhser.html

[R44] 按修改时间查找
来源：http://hz.cashguo.top/gttnzdfzwm.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtvbkemqox.html

[R45] 批量删除
来源：http://hz.c1oappe.top/gtonvpcuhu.html

find . -name "*.tmp" -delete
来源：http://hz.fengsongda.top/gthdjsakhh.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtmiouanjy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.sweek.top/gtepmmppkp.html

[R47] sed 单行替换
来源：http://hz.guannengcc.top/gtesmdmwnk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.hammf.cn/gtpptumrmy.html

[R48] awk 取指定列
来源：http://hz.zhijiandao.cn/gtccjgflsm.html

awk '{print $1, $3}' a.txt
来源：http://hz.cheryme.top/gtgdmsxujn.html

[R49] awk 带条件
来源：http://hz.shzxlz.cn/gtqfhjcvot.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zdqjudy.top/gtpinmmnca.html

[R50] awk 求和
来源：http://hz.ivvv.top/gtmvhvsbxq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.c1oappe.top/gtweyngses.html

[R51] 排序去重取前几
来源：http://hz.aizwys.cn/gttzmbhqwk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jinqigfzy.top/gtugzwmqnb.html

[R52] 统计行数
来源：http://hz.jlsjyb.cn/gtkojkelug.html

wc -l a.txt
来源：http://hz.gaohongyu789.top/gtytjaygss.html

[R53] 查看文件头与实时尾
来源：http://hz.xuetiantiany.cn/gtycmsuuxd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.nwbrower.top/gtwsmmagdm.html

[R54] 比较两个文件
来源：http://hz.aizwys.cn/gtucqueaik.html

diff a.txt b.txt
来源：http://hz.sufxvd.cn/gtrxypqnqb.html

[R55] 压缩与解压
来源：http://hz.gaohongyu789.top/gtyivxaubw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.haohaochexian.top/gtigbrxgwx.html

[R56] 远程拷贝
来源：http://hz.gogol.net.cn/gtpvkmbtjg.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtqcdtpral.html

[R57] 远程执行命令
来源：http://hz.gotoacloud.top/gteumzukyg.html

ssh user@host 'uptime'
来源：http://hz.jinghuilouyu.cn/gtjkvkiveb.html

[R58] 下载文件
来源：http://hz.redwolf501.top/gtxsmtjymb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhixingplan.top/gtpnzdncfu.html

[R59] 发 POST JSON
来源：http://hz.ydzc1.top/gtultkkcwi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shangyingyoupin.top/gtexbkzssx.html

[R60] 只看 HTTP 状态码
来源：http://hz.tanke756.top/gthooxhemi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.guowangkeji.top/gtfndqgiqu.html

[R61] 磁盘占用
来源：http://hz.shuidangran.top/gtpzdevqtv.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtafqzkyed.html

[R62] 找最占空间的文件
来源：http://hz.guannengcc.top/gtnbeliksi.html

du -ah . | sort -rh | head -10
来源：http://hz.aizwys.cn/gtphfqmfsm.html

[R63] 内存与进程
来源：http://hz.daria6918.cn/gtylblnvjw.html

free -h;  ps aux | grep nginx
来源：http://hz.snrcjt.cn/gtfecxnehm.html

[R64] 结束进程
来源：http://hz.chenjidiqi.icu/gtvcqnapae.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yongpay.top/gtvljihkvi.html

[R65] 查看端口占用
来源：http://hz.nwbrower.top/gtqmhizosc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.cashguo.top/gtzuvxcrxz.html

[R66] 定时任务
来源：http://hz.gotoacloud.top/gtybypfwpi.html

crontab -e;  crontab -l
来源：http://hz.yonumen.top/gtnblyxpil.html

[R67] 生成随机十六进制串
来源：http://hz.sxryk.cn/gttzlrbovi.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gtmyocmbll.html

[R68] 计算文件校验值
来源：http://hz.hnqzz.top/gtampftsyf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtkqthnkze.html

[R69] 生成随机密码
来源：http://hz.vqdsnc.cn/gtnbfharvy.html

head -c 16 /dev/urandom | base64
来源：http://hz.jlsjyb.cn/gtplyumexn.html

[R70] 时间戳与互转
来源：http://hz.yongpay.top/gtobbzeuuo.html

date +%s;  date -d @1700000000
来源：http://hz.wangdashe.top/gtzlrzdkxl.html

[R71] 日期格式化
来源：http://hz.ydzc1.top/gtlekwtork.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.cashguo.top/gtpudwiphq.html

[R72] 等待端口就绪
来源：http://hz.daxiang520.top/gtfewfvomg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.pycfn.com/gtnngkdgyh.html

[R73] 分割大日志
来源：http://hz.guannengcc.top/gtgpcjfrge.html

split -l 1000 big.log part_
来源：http://hz.yj202588.top/gtcfiokwpa.html

[R74] 批量重命名
来源：http://hz.smart0.xyz/gtubpcxvem.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinghuilouyu.cn/gtiifegahl.html

[R75] 导出环境变量
来源：http://hz.gotoacloud.top/gthizmpjmj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.316326.xyz/gtjvaucopq.html

[R76] 使用临时文件
来源：http://hz.hongshengwenyu.top/gtvowrqodb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtucnukbmj.html

[R77] 读取用户输入
来源：http://hz.xziqi.cn/gtkgwfolnd.html

read -rp "请输入: " ans
来源：http://hz.sweek.top/gtgxmmqlhr.html

[R78] 交互式菜单
来源：http://hz.chenzaomai.com/gthpvgdejv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jqgufenzy.top/gtacahgcmy.html

[R79] 解析命令行选项
来源：http://hz.dianchejie.cn/gtccoqfhqx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yangfankeji.com/gtwdhnjchl.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtoylooqgr.html

time ./run.sh
来源：http://hz.jlsjyb.cn/gtwrjtbgrc.html

================================================================================
来源：http://hz.hnqzz.top/gtlexeqotx.html

S. C / C++ 专题
来源：http://hz.yuxming.cn/gtusuhfyzc.html

================================================================================
来源：http://hz.jqgufenzy.top/gtftaqprfs.html

[S01] C：Hello World
来源：http://hz.hnqzz.top/gtgbtwxbxb.html

#include <stdio.h>
来源：http://hz.andypj.xyz/gtzobsslhx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhongyouzk.top/gtpyyobbfu.html

[S02] C：变量与格式化输出
来源：http://hz.316326.xyz/gtnemmvzfa.html

int a = 10; printf("%d\n", a);
来源：http://hz.vqdsnc.cn/gtujfbnvvd.html

[S03] C：读入整数
来源：http://hz.tian-w.cn/gtkgslmqic.html

int x; scanf("%d", &x);
来源：http://hz.jyoumei.cn/gtdllqhuxt.html

[S04] C：字符串复制
来源：http://hz.hywenlv.cn/gttqucrbae.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ppjwa.cn/gtohmiiawt.html

[S05] C：字符串长度
来源：http://hz.iojbl.cn/gttycirhkq.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtecgzixbz.html

[S06] C：字符串比较
来源：http://hz.xinyue.icu/gtgyhdlcfw.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangtech.top/gtqnkkotzc.html

[S07] C：数组遍历求和
来源：http://hz.zhixingplan.top/gttdnbxlmx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.tanke756.top/gtwsyjqpqk.html

[S08] C：动态内存分配与释放
来源：http://hz.yueranfly.top/gtenfepyoq.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guannengcc.top/gturogtyxf.html

[S09] C：结构体定义与初始化
来源：http://hz.fengsongda.top/gtveiypfle.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.snrcjt.cn/gtuuddahet.html

[S10] C：指针与解引用
来源：http://hz.cucudq.cn/gttqqpinvr.html

int *p = &a;  *p = 5;
来源：http://hz.ydjk.org.cn/gtzjgebbmh.html

[S11] C：逐行读文件
来源：http://hz.pycfn.com/gtcjaoxdsd.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.snrcjt.cn/gttyiqithv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.vqdsnc.cn/gtlbzchtqe.html

fclose(f);
来源：http://hz.xuetiantiany.cn/gtyvwtezoe.html

[S12] C：写文件
来源：http://hz.feifeiyinyue.top/gtxueeamlq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.zhixingplan.top/gtnptonoav.html

[S13] C：宏定义
来源：http://hz.hfpthk.cn/gtihhyyaqh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.xuanzx.com/gtokrmqpgu.html

[S14] C：枚举
来源：http://hz.jianghu66.top/gtzfjzlkwb.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.yongpay.top/gtihcgdbsa.html

[S15] C：类型转换
来源：http://hz.quarkkingdee.top/gtyagnnqzv.html

(double) a / b
来源：http://hz.cheryme.top/gtwzkxunbd.html

[S16] C：位操作置位
来源：http://hz.cucudq.cn/gtbyvbivjq.html

x |= (1 << 3);
来源：http://hz.jqgufenzy.top/gtfewfqpem.html

[S17] C：安全拼接字符串
来源：http://hz.fengsongda.top/gtdzalwhyq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.meibo888.top/gtcvwuinic.html

[S18] C：命令行参数
来源：http://hz.wangshuangyany.cn/gtphbmfhha.html

int main(int argc, char **argv)
来源：http://hz.sufxvd.cn/gtxwqlyqzf.html

[S19] C：快速排序
来源：http://hz.wangshuangyany.cn/gtsakgstae.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtrcxgsdda.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtiptpvitc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhaomingkeji.xyz/gtwhlkvxuz.html

[S21] C：字符类别判断
来源：http://hz.sweek.top/gthiogwpli.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.quarkkingdee.top/gtmfhlcfzf.html

[S22] C：字符串转数字
来源：http://hz.gzhubu.top/gtkpehxzte.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.shzxlz.cn/gtypyyijdj.html

[S23] C：随机数
来源：http://hz.hongshengwenyu.top/gtctbruzvs.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.wangshuangyany.cn/gtokzncrbe.html

[S24] C：获取本地时间
来源：http://hz.jinqigufen.top/gticrgtpjw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.ppjwa.cn/gtftxznpbx.html

[S25] C：内存拷贝
来源：http://hz.zycfv.cn/gtsrnacprr.html

memcpy(dst, src, n);
来源：http://hz.chenjidiqi.icu/gtsldecuwp.html

[S26] C：内存清零
来源：http://hz.jqgfzy.top/gtompeyiag.html

memset(a, 0, sizeof a);
来源：http://hz.mhx1999.top/gtprcachxg.html

[S27] C：定义常量
来源：http://hz.c1oappe.top/gtusvvckvb.html

const double PI = 3.14159;
来源：http://hz.chenjidiqi.icu/gtaajocpyr.html

[S28] C：静态变量
来源：http://hz.chenjidiqi.icu/gturyrxnny.html

static int counter = 0;
来源：http://hz.zhiwuduotai.top/gtqavtrilb.html

[S29] C：变参函数
来源：http://hz.sysykeji.top/gtprvpilcy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jinqigufen.top/gtewtagmpv.html

[S30] C：头文件保护
来源：http://hz.sysykeji.top/gtfdxyumud.html

#ifndef X_H
来源：http://hz.gotoacloud.top/gtiaphceuk.html

#define X_H
来源：http://hz.havefunace.top/gtonpnsboj.html

#endif
来源：http://hz.zhoulong.xyz/gtkyjqgpwd.html

[S31] C++：Hello World
来源：http://hz.shangyingyoupin.top/gtwxqjikar.html

#include <iostream>
来源：http://hz.zhoulong.xyz/gthjehvzxs.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.xziqi.cn/gttdgypdjh.html

[S32] C++：字符串
来源：http://hz.xingfuxueyuan.xyz/gtctjyoklr.html

std::string s = "hi";  s += "!";
来源：http://hz.sweek.top/gtabzabwjo.html

[S33] C++：vector 增删
来源：http://hz.jqgufenzy.top/gtaygptldn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtalcysvwv.html

[S34] C++：遍历 vector
来源：http://hz.ywan-chungtsiang.top/gtylgasbls.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yanxiufei.cn/gtdikcfqvb.html

[S35] C++：map
来源：http://hz.dashuyun.cn/gtlwlqxqyy.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtonqqfubd.html

[S36] C++：unordered_map
来源：http://hz.daxiang520.top/gtwjznadny.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hysaishi.cn/gtzlgklcrq.html

[S37] C++：set
来源：http://hz.sufxvd.cn/gtlsujacuz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.cheryme.top/gtfdpupctu.html

[S38] C++：排序
来源：http://hz.jqgufenzy.top/gtnzcsalyx.html

std::sort(v.begin(), v.end());
来源：http://hz.yangfankeji.com/gtzuqyqfhz.html

[S39] C++：自定义比较器排序
来源：http://hz.svipenyu.cn/gtfobvuzhi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.ppjwa.cn/gtmfrknmuy.html

[S40] C++：查找元素
来源：http://hz.zhixingplan.top/gtdlikoocw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.daxiang520.top/gtzyddrulp.html

[S41] C++：类与构造函数
来源：http://hz.zhaomingkeji.xyz/gtpqpcrhhi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.smart0.xyz/gtfynkfjua.html

[S42] C++：继承与虚函数
来源：http://hz.yanxiufei.cn/gtsqkygbke.html

class B : public Base { public: void f() override {} };
来源：http://hz.hfpthk.cn/gtpebexnzz.html

[S43] C++：智能指针
来源：http://hz.xingfuxueyuan.xyz/gtxelgxqig.html

auto p = std::make_unique<int>(5);
来源：http://hz.cqqwz.cn/gtixkfmmoh.html

[S44] C++：引用传参
来源：http://hz.sxryk.cn/gtzrrxyumc.html

void inc(int &x) { ++x; }
来源：http://hz.shangyingyoupin.top/gtsamzrnes.html

[S45] C++：lambda
来源：http://hz.svipenyu.cn/gtxmtxpogy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xuetiantiany.cn/gthrsyppfd.html

[S46] C++：函数模板
来源：http://hz.xziqi.cn/gtkbmanddv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.tian-w.cn/gtkpzzgpqt.html

[S47] C++：结构化绑定遍历
来源：http://hz.hnqzz.top/gtegbxrgut.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.ybcxt.top/gtfztikhbc.html

[S48] C++：逐行读文件
来源：http://hz.jqgufenzy.top/gtjpnfbfrp.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhaomingkeji.xyz/gtgllyetqw.html

while (std::getline(in, line)) { }
来源：http://hz.yangfankeji.com/gtzymxoszf.html

[S49] C++：写文件
来源：http://hz.dianchejie.cn/gtljtcqykr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.fzhhl.top/gtlfzgyqkw.html

[S50] C++：格式化数字
来源：http://hz.zhoulong.xyz/gtkciiteyr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shangyingyoupin.top/gtpiurpgar.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangtech.top/gtoszvmtey.html

static_cast<double>(a) / b
来源：http://hz.tianlin.xyz/gtyiuerige.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258888.top/gtolbdojlp.html

int size() const noexcept { return n_; }
来源：http://hz.ybcxt.top/gtgxzejjla.html

[S53] C++：移动语义
来源：http://hz.shanyushiyangtech.top/gtoonleysw.html

std::vector<int> w = std::move(v);
来源：http://hz.316326.xyz/gtirnbcpre.html

[S54] C++：异常处理
来源：http://hz.zycfv.cn/gtsmrmvlmr.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.gogol.net.cn/gtqtrsmlnv.html

[S55] C++：结构化绑定
来源：http://hz.ydjk.org.cn/gtuxwxxpea.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.dashuyun.cn/gtydiuojra.html

[S56] C++：optional
来源：http://hz.sufxvd.cn/gtfjzseubc.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.shzxlz.cn/gteqopfbfm.html

[S57] C++：编译期常量
来源：http://hz.smart0.xyz/gtngpoglzk.html

constexpr int N = 10;
来源：http://hz.ppjwa.cn/gtyqwiecbb.html

[S58] C++：命名空间
来源：http://hz.sxryk.cn/gtncvoqqng.html

namespace ns { int f() { return 1; } }
来源：http://hz.meibo888.top/gtbkjkzeqb.html

[S59] C++：静态断言
来源：http://hz.ydjk.org.cn/gtcsixzask.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtckinsqeb.html

[S60] C++：遍历并删除元素
来源：http://hz.316326.xyz/gtsesuqgwi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.jinqigfzy.top/gtuenntrku.html

================================================================================
来源：http://hz.yj20258888.top/gtadfwvfna.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.ivvv.top/gtwynvkcel.html

================================================================================
来源：http://hz.jyoumei.cn/gtioxxoabk.html

[T01] Kotlin：Hello World
来源：http://hz.birdmap.top/gtodzhlldh.html

println("Hello")
来源：http://hz.jqgfzy.top/gtmxsajtlg.html

[T02] Kotlin：变量
来源：http://hz.yonumen.top/gtbcmyexbc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.0kj1m.cn/gtyeylvezc.html

[T03] Kotlin：字符串模板
来源：http://hz.hfpthk.cn/gtdpdmemky.html

"值: $b"
来源：http://hz.jiagoushi.top/gtaqsufxrm.html

[T04] Kotlin：空安全
来源：http://hz.9152youxi.cn/gtangskwzs.html

val n: String? = null;  n?.length
来源：http://hz.dianchejie.cn/gtsuuultlp.html

[T05] Kotlin：when 表达式
来源：http://hz.yangfankeji.com/gtfujglsye.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.sysykeji.top/gtoimejrlz.html

[T06] Kotlin：集合映射
来源：http://hz.ydzc1.top/gtysmzqagx.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.havefunace.top/gtvjixoaki.html

[T07] Kotlin：集合过滤
来源：http://hz.wangshuangyany.cn/gtyxbbnboz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.meibo888.top/gtdkvhryjt.html

[T08] Kotlin：数据类
来源：http://hz.zhongyouzk.top/gtqmfryzti.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxuanxn.top/gtjuwgqzzq.html

[T09] Kotlin：扩展函数
来源：http://hz.ybcxt.top/gtsgovxtnk.html

fun String.exclaim() = this + "!"
来源：http://hz.tian-w.cn/gtwadxnvbw.html

[T10] Kotlin：默认参数
来源：http://hz.zhijiandao.cn/gtcgislonb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.zhoulong.xyz/gtdxdorsve.html

[T11] Kotlin：协程
来源：http://hz.cheryme.top/gthnsrmxql.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.jinyuanbaomall.cn/gtymphesiu.html

[T12] Kotlin：解构声明
来源：http://hz.c1oappe.top/gthjkrhdvm.html

val (a, b) = Pair(1, 2)
来源：http://hz.dashuyun.cn/gtfunwxten.html


<!-- 参考信息 -->