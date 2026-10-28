代发 wailian999

case "$1" in
来源：http://hz.aibaodan.cn/gtqisuaahy.html

start) echo "启动" ;;
来源：http://hz.gaohongyu789.top/gtzqtwhxmc.html

stop)  echo "停止" ;;
来源：http://hz.shuidangran.top/gtcuknvmlo.html

*)     echo "未知命令" ;;
来源：http://hz.chenlongwang.top/gtpabjkoqz.html

esac
来源：http://hz.aibaodan.cn/gtgxswlpfr.html

[R12] for 遍历文件
来源：http://hz.jinghuilouyu.cn/gtxfbbydor.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ivvv.top/gtqznldclb.html

[R13] for 计数循环
来源：http://hz.gotoacloud.top/gtsxyjwxoa.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yj20258888.top/gtezfcbbox.html

[R14] C 风格 for
来源：http://hz.chenzaomai.com/gtvotoshbc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.daxiang520.top/gtzisfnsck.html

[R15] while 逐行读文件
来源：http://hz.andypj.xyz/gtzfowjqrp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yongpay.top/gtelxkoirp.html

[R16] until 等待条件
来源：http://hz.jinqigfzy.top/gtudhevajo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhengqikj.top/gtjrlswonn.html

[R17] 数组定义与取值
来源：http://hz.9152youxi.cn/gtvphrsxaj.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jianghu66.top/gtuuadzwhv.html

[R18] 遍历数组
来源：http://hz.yj202588.top/gthhjdzslj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnqzz.top/gtklvfhpjq.html

[R19] 数组长度
来源：http://hz.xuetiantiany.cn/gtmmxtffca.html

echo "${#arr[@]}"
来源：http://hz.zhaomingkeji.xyz/gtgxcgbvrk.html

[R20] 关联数组（字典）
来源：http://hz.gogol.net.cn/gtiotddgoc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.svipenyu.cn/gtxqtgnsgm.html

[R21] 字符串长度
来源：http://hz.cheryme.top/gtzqtkfwxj.html

echo "${#s}"
来源：http://hz.ehwqpu.com/gtibddscbh.html

[R22] 截取子串
来源：http://hz.nanxuanxn.top/gtazoddwro.html

echo "${s:0:5}"
来源：http://hz.haohaochexian.top/gtkdcosejr.html

[R23] 字符串替换
来源：http://hz.snrcjt.cn/gtnvduxbcd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jiagoushi.top/gtyrzijrny.html

[R24] 大小写转换
来源：http://hz.52xcode.cn/gtsjexkjij.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hysaishi.cn/gtwvzosogv.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhongyouzk.top/gtmkpkkfne.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.hnqzz.top/gtfgjwejnd.html

[R26] 命令替换
来源：http://hz.nanxinkj.top/gtqitfekjs.html

now=$(date +%F); echo "$now"
来源：http://hz.mhx1999.top/gtipzguirl.html

[R27] 算术展开
来源：http://hz.dianchejie.cn/gtzwcijuma.html

echo $((1 + 2 * 3))
来源：http://hz.gogol.net.cn/gtiogzjmpe.html

[R28] 浮点运算
来源：http://hz.jqgufenzy.top/gthxjvctfq.html

echo "scale=2; 10/3" | bc
来源：http://hz.ppjwa.cn/gthkmhgssp.html

[R29] 定义函数
来源：http://hz.iojbl.cn/gtqqbhkspy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.ivvv.top/gtginqoari.html

[R30] 函数返回状态码
来源：http://hz.zhaomingkeji.xyz/gtkaamoard.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xinyue.icu/gtqsyrreth.html

[R31] 局部变量
来源：http://hz.mhx1999.top/gtfbkwnsvn.html

f() { local x=1; echo "$x"; }
来源：http://hz.wangshuangyany.cn/gthxtvbwlp.html

[R32] 参数个数校验
来源：http://hz.daxiang520.top/gtqgghypxs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yueranfly.top/gtpsuaqzig.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtymiarqnw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gtgkemsonb.html

[R34] 退出时清理
来源：http://hz.bjfxy.top/gtsrrzcdjl.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.iojbl.cn/gtcveyqqnz.html

[R35] 后台执行并等待
来源：http://hz.shangyingyoupin.top/gtyzpsdewc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hongshengwenyu.top/gtnmjrhguk.html

[R36] 并发执行多个任务
来源：http://hz.chenzaomai.com/gtcwikcpzo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.chenlongwang.top/gtwyldhdwu.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtflycuqwc.html

files=$(ls -1)
来源：http://hz.svipenyu.cn/gtsdqfsfjm.html

[R38] 管道串联
来源：http://hz.ppjwa.cn/gtceqxrpfa.html

cat a.txt | grep -i error | wc -l
来源：http://hz.hywenlv.cn/gtrvlqjxbg.html

[R39] 重定向标准输出与错误
来源：http://hz.cheryme.top/gtfdzwengo.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangtech.top/gtqpsrxidm.html

[R40] 追加写日志
来源：http://hz.0kj1m.cn/gtzgyomupq.html

echo "log" >> out.log
来源：http://hz.havefunace.top/gtzadhglom.html

[R41] 丢弃输出
来源：http://hz.meibo888.top/gtqwmxusxd.html

cmd >/dev/null 2>&1
来源：http://hz.jqgfzy.top/gtldhzupow.html

[R42] 输入重定向
来源：http://hz.aizwys.cn/gtoqydldgl.html

wc -l < a.txt
来源：http://hz.jqgufenzy.top/gtiesqihlu.html

[R43] 按名字查找文件
来源：http://hz.pengpengdd.cyou/gtamyigcdr.html

find . -name "*.log" -type f
来源：http://hz.hnxiangtu.top/gtyyqgflcm.html

[R44] 按修改时间查找
来源：http://hz.hnqzz.top/gtftrobtyn.html

find . -mtime -7 -type f
来源：http://hz.316326.xyz/gtrhprxkdj.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtzsgicnbr.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258.top/gttzidgwlc.html

[R46] 递归替换文件内容
来源：http://hz.shanyushiyangkeji.top/gtxaekzgax.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.shangyingyoupin.top/gtalkhexdc.html

[R47] sed 单行替换
来源：http://hz.chenjidiqi.icu/gtbcpjrlhl.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydzc1.top/gteevdhphc.html

[R48] awk 取指定列
来源：http://hz.yanxiufei.cn/gtutmvmgzt.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtzhbmuhuz.html

[R49] awk 带条件
来源：http://hz.jqgufenzy.top/gtfneuzykw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zycfv.cn/gtwlriweox.html

[R50] awk 求和
来源：http://hz.zycfv.cn/gtewahlfvy.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hammf.cn/gtewgmodvb.html

[R51] 排序去重取前几
来源：http://hz.daxiang520.top/gtombkartq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.shanyushiyangkeji.top/gtexjlioyo.html

[R52] 统计行数
来源：http://hz.jinyuanbaomall.cn/gtanmcwqbk.html

wc -l a.txt
来源：http://hz.zhijiandao.cn/gtzfjbhxqd.html

[R53] 查看文件头与实时尾
来源：http://hz.tian-w.cn/gtnrmkvsyj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jlsjyb.cn/gtdbcjdvbc.html

[R54] 比较两个文件
来源：http://hz.nwbrower.top/gtmkvsdlvq.html

diff a.txt b.txt
来源：http://hz.zhiwuduotai.top/gtpregehxy.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtnydowcon.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pengpengdd.cyou/gtglrtsiee.html

[R56] 远程拷贝
来源：http://hz.aizwys.cn/gtsdkvzzzg.html

scp file user@host:/path/
来源：http://hz.hammf.cn/gtnkpkneti.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtvdzjudpt.html

ssh user@host 'uptime'
来源：http://hz.ydjk.org.cn/gtzkpuepcl.html

[R58] 下载文件
来源：http://hz.haohaochexian.top/gtgmydjajy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinyuanbaomall.cn/gtqxgoousj.html

[R59] 发 POST JSON
来源：http://hz.xuanzx.com/gtcpraxetr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.zdqjudy.top/gthtnhxuxh.html

[R60] 只看 HTTP 状态码
来源：http://hz.aibaodan.cn/gteuhcbbri.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.xingfuxueyuan.xyz/gtqhqfgzub.html

[R61] 磁盘占用
来源：http://hz.zhiwuduotai.top/gtthmkwyeg.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gtqxhvrlez.html

[R62] 找最占空间的文件
来源：http://hz.yuxming.cn/gtmldabwyc.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gtngupestk.html

[R63] 内存与进程
来源：http://hz.shanyushiyangkeji.top/gtcbpjotfv.html

free -h;  ps aux | grep nginx
来源：http://hz.xuanzx.com/gtoqarjytc.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtgmzjlibb.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinyuanbaomall.cn/gtvxfypucj.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtqohipeyn.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sxryk.cn/gtgyrjlhux.html

[R66] 定时任务
来源：http://hz.shanyushiyangtech.top/gtjvlggxuf.html

crontab -e;  crontab -l
来源：http://hz.guowangkeji.top/gtwwiorpqv.html

[R67] 生成随机十六进制串
来源：http://hz.xuetiantiany.cn/gtynzdjtoc.html

openssl rand -hex 16
来源：http://hz.tanke756.top/gtwllbndaa.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtvzkicgng.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.tanke756.top/gtjnwfqwjf.html

[R69] 生成随机密码
来源：http://hz.ivvv.top/gtvgnpzjuw.html

head -c 16 /dev/urandom | base64
来源：http://hz.jyoumei.cn/gtmkiquuty.html

[R70] 时间戳与互转
来源：http://hz.aibaodan.cn/gtsdqtzozt.html

date +%s;  date -d @1700000000
来源：http://hz.ehwqpu.com/gtcsuqjryc.html

[R71] 日期格式化
来源：http://hz.hnqzz.top/gtjulroohc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtuxwuxedz.html

[R72] 等待端口就绪
来源：http://hz.yj20258888.top/gteqvxbizc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydzc1.top/gtagpkuwoj.html

[R73] 分割大日志
来源：http://hz.redwolf501.top/gttvltmrxp.html

split -l 1000 big.log part_
来源：http://hz.9152youxi.cn/gtxmmfkdtf.html

[R74] 批量重命名
来源：http://hz.jyoumei.cn/gtpjolcvoh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yongpay.top/gthujmmike.html

[R75] 导出环境变量
来源：http://hz.hnqzz.top/gtnaxqddyr.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.chenlongwang.top/gtrzffsogw.html

[R76] 使用临时文件
来源：http://hz.yangfankeji.com/gtxdpzcisk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yangfankeji.com/gtertgqigh.html

[R77] 读取用户输入
来源：http://hz.hfpthk.cn/gttuoqqayx.html

read -rp "请输入: " ans
来源：http://hz.birdmap.top/gtusatxcmp.html

[R78] 交互式菜单
来源：http://hz.xingfuxueyuan.xyz/gtqsouuzgy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hongshengwenyu.top/gtqreadpyv.html

[R79] 解析命令行选项
来源：http://hz.zhixingplan.top/gtewbbugxn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangkeji.top/gthddyhrtc.html

[R80] 查看脚本执行耗时
来源：http://hz.jinqigfzy.top/gtpcncqvlc.html

time ./run.sh
来源：http://hz.ybcxt.top/gtmppcshvb.html

================================================================================
来源：http://hz.tanke756.top/gtrhyxvjcg.html

S. C / C++ 专题
来源：http://hz.shanyushiyangkeji.top/gtjjujdxjg.html

================================================================================
来源：http://hz.redwolf501.top/gthbwgxpuj.html

[S01] C：Hello World
来源：http://hz.dianchejie.cn/gtvyxrtcsq.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtbafuzjkm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.pengpengdd.cyou/gtaluwthup.html

[S02] C：变量与格式化输出
来源：http://hz.gaohongyu789.top/gtrwgyibdk.html

int a = 10; printf("%d\n", a);
来源：http://hz.zhixingplan.top/gtbxafcbnb.html

[S03] C：读入整数
来源：http://hz.ydjk.org.cn/gtczufuhqd.html

int x; scanf("%d", &x);
来源：http://hz.guannengcc.top/gtkkomcihv.html

[S04] C：字符串复制
来源：http://hz.fzhhl.top/gtmokqaknj.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.cqqwz.cn/gtlcdbjkzh.html

[S05] C：字符串长度
来源：http://hz.birdmap.top/gtpdlsspdk.html

strlen(s)
来源：http://hz.meibo888.top/gtsvccafnn.html

[S06] C：字符串比较
来源：http://hz.yj20258888.top/gtkiicvnuy.html

strcmp(a, b) == 0
来源：http://hz.chenzaomai.com/gtwckuxbkq.html

[S07] C：数组遍历求和
来源：http://hz.redwolf501.top/gtwptgaqzm.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtdhsyvini.html

[S08] C：动态内存分配与释放
来源：http://hz.zhoulong.xyz/gtjcekqrpd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.shzxlz.cn/gtvousvzko.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtmhgypxco.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jqgfzy.top/gtjonasdoo.html

[S10] C：指针与解引用
来源：http://hz.hywenlv.cn/gtkbdfxodx.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtnwqjrgco.html

[S11] C：逐行读文件
来源：http://hz.xylfe.cn/gtwlqgtdke.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yj202588.top/gtpyfwjkjb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenjidiqi.icu/gtsdolpejm.html

fclose(f);
来源：http://hz.havefunace.top/gttnfzjkli.html

[S12] C：写文件
来源：http://hz.gzhubu.top/gtjrzdxrrl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gogol.net.cn/gtctbhaysy.html

[S13] C：宏定义
来源：http://hz.andypj.xyz/gtdwodannw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.feifeiyinyue.top/gtszlmtqoa.html

[S14] C：枚举
来源：http://hz.aibaodan.cn/gtrfuygkwj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cucudq.cn/gtdclxabdm.html

[S15] C：类型转换
来源：http://hz.nanxuanxn.top/gtqxpmatue.html

(double) a / b
来源：http://hz.mhx1999.top/gtnvozibpn.html

[S16] C：位操作置位
来源：http://hz.52xcode.cn/gtsfqygopl.html

x |= (1 << 3);
来源：http://hz.birdmap.top/gtkrwntpep.html

[S17] C：安全拼接字符串
来源：http://hz.wangshuangyany.cn/gtreakvbna.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.quarkkingdee.top/gtprkbkkpu.html

[S18] C：命令行参数
来源：http://hz.guowangkeji.top/gtxpsgesav.html

int main(int argc, char **argv)
来源：http://hz.shanyushiyangkeji.top/gtxunztyna.html

[S19] C：快速排序
来源：http://hz.yj20258.top/gtdljlxsdl.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtfcutiywu.html

[S20] C：二分查找
来源：http://hz.gogol.net.cn/gtxpifywkb.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.9152youxi.cn/gtnuqukjtv.html

[S21] C：字符类别判断
来源：http://hz.nwbrower.top/gtfwbmfbel.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.haohaochexian.top/gtebyaotos.html

[S22] C：字符串转数字
来源：http://hz.xziqi.cn/gtbzkvpwkq.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gtvqmengls.html

[S23] C：随机数
来源：http://hz.smart0.xyz/gtqeqyuesr.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cucudq.cn/gtasauxqek.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gtqlrpntic.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cucudq.cn/gtuzytgmwj.html

[S25] C：内存拷贝
来源：http://hz.xuanzx.com/gtxdsiskim.html

memcpy(dst, src, n);
来源：http://hz.xinyue.icu/gtxkdmglkh.html

[S26] C：内存清零
来源：http://hz.jlsjyb.cn/gtmxcitifd.html

memset(a, 0, sizeof a);
来源：http://hz.jqgufenzy.top/gtxxaldrig.html

[S27] C：定义常量
来源：http://hz.sufxvd.cn/gtqzxrqjau.html

const double PI = 3.14159;
来源：http://hz.316326.xyz/gtetjvcmhf.html

[S28] C：静态变量
来源：http://hz.zhixingplan.top/gtkaomnuhe.html

static int counter = 0;
来源：http://hz.smart0.xyz/gtjcqtcrbd.html

[S29] C：变参函数
来源：http://hz.jiagoushi.top/gthqyzuzxm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.zhiwuduotai.top/gtgxbbdkvc.html

[S30] C：头文件保护
来源：http://hz.chenlongwang.top/gtilenvpch.html

#ifndef X_H
来源：http://hz.hysaishi.cn/gtawplcvft.html

#define X_H
来源：http://hz.xylfe.cn/gtdtqbdrpm.html

#endif
来源：http://hz.pengpengdd.cyou/gtpxvefbyd.html

[S31] C++：Hello World
来源：http://hz.xuanzx.com/gtzbvhwqoj.html

#include <iostream>
来源：http://hz.316326.xyz/gtbktoqggy.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ywan-chungtsiang.top/gtobzyzery.html

[S32] C++：字符串
来源：http://hz.guannengcc.top/gtgppxbwgl.html

std::string s = "hi";  s += "!";
来源：http://hz.ppjwa.cn/gtfmsiylgo.html

[S33] C++：vector 增删
来源：http://hz.aibaodan.cn/gtcgvhmmsz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtievqoqqz.html

[S34] C++：遍历 vector
来源：http://hz.cdnleiting.top/gtjwwpjqdw.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dianchejie.cn/gtdppjqxfl.html

[S35] C++：map
来源：http://hz.aizwys.cn/gtqpqvzoaf.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtwpoyffdg.html

[S36] C++：unordered_map
来源：http://hz.vqdsnc.cn/gtzrsvtnou.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtswnqlgml.html

[S37] C++：set
来源：http://hz.hnxiangtu.top/gtdbnastmk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.zhiwuduotai.top/gtkrzbmihq.html

[S38] C++：排序
来源：http://hz.bjfxy.top/gtzahsqfqz.html

std::sort(v.begin(), v.end());
来源：http://hz.316326.xyz/gtgdkwdpax.html

[S39] C++：自定义比较器排序
来源：http://hz.zhaomingkeji.xyz/gtjncitxsd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.vqdsnc.cn/gtnelivlns.html

[S40] C++：查找元素
来源：http://hz.cqqwz.cn/gtserswkcx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.hnxiangtu.top/gtilebjnmk.html

[S41] C++：类与构造函数
来源：http://hz.xinyue.icu/gtzvqwsfvf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.zhoulong.xyz/gtlilmihol.html

[S42] C++：继承与虚函数
来源：http://hz.bjfxy.top/gtzsshsvgt.html

class B : public Base { public: void f() override {} };
来源：http://hz.jiagoushi.top/gtajyzwava.html

[S43] C++：智能指针
来源：http://hz.zhengqikj.top/gtgnewntew.html

auto p = std::make_unique<int>(5);
来源：http://hz.cashguo.top/gtyhoyfpfu.html

[S44] C++：引用传参
来源：http://hz.jinqigufen.top/gtzycoxowx.html

void inc(int &x) { ++x; }
来源：http://hz.cucudq.cn/gtcvymspxd.html

[S45] C++：lambda
来源：http://hz.xinyue.icu/gtzynkesxi.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zycfv.cn/gtlbevwpny.html

[S46] C++：函数模板
来源：http://hz.guannengcc.top/gtxcirnvgr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shuidangran.top/gtjsnvjndf.html

[S47] C++：结构化绑定遍历
来源：http://hz.cheryme.top/gtsszlxlpm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jinyuanbaomall.cn/gtzqlspkwo.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gtjmphihmi.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.zhongyouzk.top/gtompysfnb.html

while (std::getline(in, line)) { }
来源：http://hz.zhixingplan.top/gtsnayrdwk.html

[S49] C++：写文件
来源：http://hz.fengsongda.top/gtxzujrwyu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xingfuxueyuan.xyz/gtlstruubg.html

[S50] C++：格式化数字
来源：http://hz.cheryme.top/gtgjeasgsb.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.chenzaomai.com/gtlfqtcjci.html

[S51] C++：显式类型转换
来源：http://hz.shanyushiyangkeji.top/gthbnenswj.html

static_cast<double>(a) / b
来源：http://hz.tanke756.top/gtkancluaa.html

[S52] C++：const 与 noexcept
来源：http://hz.zhaomingkeji.xyz/gtqphualdl.html

int size() const noexcept { return n_; }
来源：http://hz.jyoumei.cn/gtbkajhtle.html

[S53] C++：移动语义
来源：http://hz.mhx1999.top/gtcjklfarw.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtqhkztgjm.html

[S54] C++：异常处理
来源：http://hz.yuanzhike.top/gtjyiehuej.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.hnxiangtu.top/gtpeodjvxc.html

[S55] C++：结构化绑定
来源：http://hz.feifeiyinyue.top/gtxkqojcef.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yonumen.top/gtkopdxike.html

[S56] C++：optional
来源：http://hz.cashguo.top/gtldyudosg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.aibaodan.cn/gtoiicghax.html

[S57] C++：编译期常量
来源：http://hz.ydzc1.top/gtmajkmesm.html

constexpr int N = 10;
来源：http://hz.cucudq.cn/gtnuzvoovl.html

[S58] C++：命名空间
来源：http://hz.chenzaomai.com/gtwnganrgk.html

namespace ns { int f() { return 1; } }
来源：http://hz.pengpengdd.cyou/gtdoabsmdn.html

[S59] C++：静态断言
来源：http://hz.guowangkeji.top/gtmpczdgva.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.jinqigufen.top/gtjjsuyjqd.html

[S60] C++：遍历并删除元素
来源：http://hz.feifeiyinyue.top/gtaesrnoon.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.guowangkeji.top/gtkhvqezhb.html

================================================================================
来源：http://hz.zycfv.cn/gtajaerxcr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.daria6918.cn/gtnuvfsuep.html

================================================================================
来源：http://hz.jinqigufen.top/gtnuiegdky.html

[T01] Kotlin：Hello World
来源：http://hz.daxiang520.top/gtawfjqrve.html

println("Hello")
来源：http://hz.guowangkeji.top/gtqxlntgfu.html

[T02] Kotlin：变量
来源：http://hz.ybcxt.top/gtcoamkjfz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shangyingyoupin.top/gtftwykdal.html

[T03] Kotlin：字符串模板
来源：http://hz.xuetiantiany.cn/gtqfpcgyuv.html

"值: $b"
来源：http://hz.9152youxi.cn/gtqqytbkok.html

[T04] Kotlin：空安全
来源：http://hz.pycfn.com/gtewhnyfuv.html

val n: String? = null;  n?.length
来源：http://hz.jyoumei.cn/gtntcdvhfn.html

[T05] Kotlin：when 表达式
来源：http://hz.hywenlv.cn/gtpvhahcmc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.vqdsnc.cn/gtkhcplmqo.html

[T06] Kotlin：集合映射
来源：http://hz.ivvv.top/gtfotcrynv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.cucudq.cn/gtwlolcysy.html

[T07] Kotlin：集合过滤
来源：http://hz.redwolf501.top/gtobulwoyr.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.cucudq.cn/gtbhjxgxbd.html

[T08] Kotlin：数据类
来源：http://hz.jinqigfzy.top/gtnbdbcbmy.html

data class User(val name: String, val age: Int)
来源：http://hz.xylfe.cn/gtolapimzu.html

[T09] Kotlin：扩展函数
来源：http://hz.daria6918.cn/gtepkqpcgi.html

fun String.exclaim() = this + "!"
来源：http://hz.yj20258.top/gtuidqaovq.html

[T10] Kotlin：默认参数
来源：http://hz.hywenlv.cn/gttbwpcbte.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.xuetiantiany.cn/gtvlqifzoy.html

[T11] Kotlin：协程
来源：http://hz.316326.xyz/gtcxxsfwhd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yueranfly.top/gtvtijxwmu.html

[T12] Kotlin：解构声明
来源：http://hz.quarkkingdee.top/gtnwswfefk.html

val (a, b) = Pair(1, 2)
来源：http://hz.yangfankeji.com/gtqhibbatd.html


<!-- 参考信息 -->