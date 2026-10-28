代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jianghu66.top/gtngysrdpd.html

[R10] 正则匹配
来源：http://hz.chenjidiqi.icu/gtozvswaiq.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.jinqigfzy.top/gtqudkkbhu.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtnymorzvm.html

case "$1" in
来源：http://hz.sysykeji.top/gtgmngeoci.html

start) echo "启动" ;;
来源：http://hz.yuanzhike.top/gtchloayuq.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtlwrekmdk.html

*)     echo "未知命令" ;;
来源：http://hz.andypj.xyz/gtmthefmdj.html

esac
来源：http://hz.jiagoushi.top/gtydmknmpb.html

[R12] for 遍历文件
来源：http://hz.yvedp.cn/gtqaqhmofn.html

for f in *.txt; do echo "$f"; done
来源：http://hz.dashuyun.cn/gttgyxoxvr.html

[R13] for 计数循环
来源：http://hz.nwbrower.top/gtqgodvdkr.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xuanzx.com/gttbxywssz.html

[R14] C 风格 for
来源：http://hz.hammf.cn/gtqjmveqpy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.bjfxy.top/gtlhdvrdyi.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gtijxgchbh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gtmcnywrey.html

[R16] until 等待条件
来源：http://hz.tanke756.top/gtmsqfimzu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shzxlz.cn/gtkxjeqjcg.html

[R17] 数组定义与取值
来源：http://hz.zhiwuduotai.top/gtukrivgzb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.andypj.xyz/gtpgvqzdhx.html

[R18] 遍历数组
来源：http://hz.smart0.xyz/gtxzdlcarp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.fengsongda.top/gtmhzgntvj.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gtvuoiqmdo.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gthviauauw.html

[R20] 关联数组（字典）
来源：http://hz.vqdsnc.cn/gtvgfceqye.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shanyushiyangkeji.top/gtjdmvxyhi.html

[R21] 字符串长度
来源：http://hz.yj202588.top/gtodwvygij.html

echo "${#s}"
来源：http://hz.0kj1m.cn/gtkjmvvoel.html

[R22] 截取子串
来源：http://hz.tianlin.xyz/gtnfckabwt.html

echo "${s:0:5}"
来源：http://hz.ybcxt.top/gttjzcwbtg.html

[R23] 字符串替换
来源：http://hz.chenzaomai.com/gtscetcpaz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nanxuanxn.top/gtlgxdgero.html

[R24] 大小写转换
来源：http://hz.chenzaomai.com/gtjtkclaxw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.shzxlz.cn/gtrflymvod.html

[R25] 去后缀 / 去前缀
来源：http://hz.yueranfly.top/gtmtlckjdt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jlsjyb.cn/gthrljgoao.html

[R26] 命令替换
来源：http://hz.yj202588.top/gtaighuytz.html

now=$(date +%F); echo "$now"
来源：http://hz.shuidangran.top/gtpehjxias.html

[R27] 算术展开
来源：http://hz.yvedp.cn/gtooylgvhl.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtqtocwpyg.html

[R28] 浮点运算
来源：http://hz.hammf.cn/gtrioxtyxn.html

echo "scale=2; 10/3" | bc
来源：http://hz.xylfe.cn/gtytwtpxsq.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtkiqfywau.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.chenzaomai.com/gtqqsvhgzs.html

[R30] 函数返回状态码
来源：http://hz.jianghu66.top/gtcbljkajd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.smart0.xyz/gtchkwgnzv.html

[R31] 局部变量
来源：http://hz.zycfv.cn/gtjtfpqpjc.html

f() { local x=1; echo "$x"; }
来源：http://hz.tian-w.cn/gtdmeweirl.html

[R32] 参数个数校验
来源：http://hz.yongpay.top/gtmdoblopl.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.nanxuanxn.top/gtawaxqjyg.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtjoblcwzm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.fengsongda.top/gtgutvkmeo.html

[R34] 退出时清理
来源：http://hz.fengsongda.top/gtmhkdolcc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinghuilouyu.cn/gtwihdnnwb.html

[R35] 后台执行并等待
来源：http://hz.aizwys.cn/gtnqbrclwb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tian-w.cn/gtryvnkpdx.html

[R36] 并发执行多个任务
来源：http://hz.hongshengwenyu.top/gtkqufundv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.nwbrower.top/gtzricvdmh.html

[R37] 把输出赋给变量
来源：http://hz.hnqzz.top/gtddkqzgdv.html

files=$(ls -1)
来源：http://hz.ywan-chungtsiang.top/gtuikmxloz.html

[R38] 管道串联
来源：http://hz.xuanzx.com/gtauelqxsl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yonumen.top/gtiklvqpzg.html

[R39] 重定向标准输出与错误
来源：http://hz.nwbrower.top/gtohahwixk.html

cmd > out.log 2>&1
来源：http://hz.hywenlv.cn/gtirzgcbxz.html

[R40] 追加写日志
来源：http://hz.jianghu66.top/gttkbnaqpz.html

echo "log" >> out.log
来源：http://hz.meibo888.top/gtfdawhrxp.html

[R41] 丢弃输出
来源：http://hz.daria6918.cn/gtodrgdlld.html

cmd >/dev/null 2>&1
来源：http://hz.jqgufenzy.top/gtugizdycf.html

[R42] 输入重定向
来源：http://hz.ydjk.org.cn/gtsbjneywv.html

wc -l < a.txt
来源：http://hz.hfpthk.cn/gtjryvvqjl.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtmhcsbgrh.html

find . -name "*.log" -type f
来源：http://hz.gaohongyu789.top/gtqgbcctyr.html

[R44] 按修改时间查找
来源：http://hz.haohaochexian.top/gtdrusdyya.html

find . -mtime -7 -type f
来源：http://hz.zdqjudy.top/gtkpwynber.html

[R45] 批量删除
来源：http://hz.quarkkingdee.top/gtidknlwvv.html

find . -name "*.tmp" -delete
来源：http://hz.pengpengdd.cyou/gtapyqrooh.html

[R46] 递归替换文件内容
来源：http://hz.chenzaomai.com/gtowhrihkf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.tianlin.xyz/gtovrxslxn.html

[R47] sed 单行替换
来源：http://hz.daria6918.cn/gtdfigtcvi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.nanxuanxn.top/gtxnasgydd.html

[R48] awk 取指定列
来源：http://hz.c1oappe.top/gtdffysygf.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhengqikj.top/gtvswcvxli.html

[R49] awk 带条件
来源：http://hz.9152youxi.cn/gtaunqankj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gaohongyu789.top/gtalioxqjk.html

[R50] awk 求和
来源：http://hz.pycfn.com/gthyotcbdc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.wangdashe.top/gtkdflemvo.html

[R51] 排序去重取前几
来源：http://hz.zhengqikj.top/gtmooeleyq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.fzhhl.top/gtijfzneww.html

[R52] 统计行数
来源：http://hz.tianlin.xyz/gtwzkhrflt.html

wc -l a.txt
来源：http://hz.tian-w.cn/gteyltvfrh.html

[R53] 查看文件头与实时尾
来源：http://hz.yonumen.top/gtubmafjzp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.birdmap.top/gtpgxrzlqm.html

[R54] 比较两个文件
来源：http://hz.mhx1999.top/gtwojlplfq.html

diff a.txt b.txt
来源：http://hz.jiagoushi.top/gtyjiubucu.html

[R55] 压缩与解压
来源：http://hz.jlsjyb.cn/gtxzjgsjmj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.gotoacloud.top/gtnqcifeyc.html

[R56] 远程拷贝
来源：http://hz.yanxiufei.cn/gtsasszjhn.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtwjrqmpty.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gtrouyyppe.html

ssh user@host 'uptime'
来源：http://hz.gaohongyu789.top/gtnnvxgjdi.html

[R58] 下载文件
来源：http://hz.ybcxt.top/gtqvaddtyk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.shangyingyoupin.top/gtxfqyslpf.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gthkvmyugz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gotoacloud.top/gtxrwsjqrz.html

[R60] 只看 HTTP 状态码
来源：http://hz.ydjk.org.cn/gthzggrxvk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.zhixingplan.top/gtbxpwxaza.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gtmbtmeckh.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtoeduebwm.html

[R62] 找最占空间的文件
来源：http://hz.hnxiangtu.top/gtnsytnpxd.html

du -ah . | sort -rh | head -10
来源：http://hz.dashuyun.cn/gtlgmoutil.html

[R63] 内存与进程
来源：http://hz.cheryme.top/gtsayjtydh.html

free -h;  ps aux | grep nginx
来源：http://hz.daxiang520.top/gtobojlqlp.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gtmkmnmvwk.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuetiantiany.cn/gtmcymmcup.html

[R65] 查看端口占用
来源：http://hz.chenjidiqi.icu/gtslfountx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yangfankeji.com/gtzqqtwply.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gtxrkhhgjz.html

crontab -e;  crontab -l
来源：http://hz.chenzaomai.com/gtzdzhkyxk.html

[R67] 生成随机十六进制串
来源：http://hz.redwolf501.top/gtdrespdfa.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gtcvrwghtu.html

[R68] 计算文件校验值
来源：http://hz.guowangkeji.top/gtselpubpo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.ywan-chungtsiang.top/gtcgzvrlvo.html

[R69] 生成随机密码
来源：http://hz.tanke756.top/gttvuoxkph.html

head -c 16 /dev/urandom | base64
来源：http://hz.gzhubu.top/gtetilknsm.html

[R70] 时间戳与互转
来源：http://hz.chenzaomai.com/gtzqojtitx.html

date +%s;  date -d @1700000000
来源：http://hz.gzhubu.top/gtpcdfvgda.html

[R71] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtkwitbciy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.meibo888.top/gtnnsfdkgv.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtpurquszh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtusriswya.html

[R73] 分割大日志
来源：http://hz.cheryme.top/gtwzwgvxka.html

split -l 1000 big.log part_
来源：http://hz.hnxiangtu.top/gtezxqujnk.html

[R74] 批量重命名
来源：http://hz.sufxvd.cn/gtmqtucfaa.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtqbaqyugr.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtikolnmwi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.9152youxi.cn/gtivnpwfmk.html

[R76] 使用临时文件
来源：http://hz.c1oappe.top/gtzwxjrxyu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xinyue.icu/gtegiekekg.html

[R77] 读取用户输入
来源：http://hz.tian-w.cn/gtytcyffck.html

read -rp "请输入: " ans
来源：http://hz.hammf.cn/gtuugdshcs.html

[R78] 交互式菜单
来源：http://hz.xuanzx.com/gtcihhbouu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuxming.cn/gtddphevid.html

[R79] 解析命令行选项
来源：http://hz.0kj1m.cn/gtdwtbcnaw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.redwolf501.top/gtfvujshfx.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gteyhznltu.html

time ./run.sh
来源：http://hz.316326.xyz/gtdsbglgle.html

================================================================================
来源：http://hz.aibaodan.cn/gthkgvyzsl.html

S. C / C++ 专题
来源：http://hz.kuanghao11.cn/gtkcikaoeo.html

================================================================================
来源：http://hz.jlsjyb.cn/gtmtbwcroe.html

[S01] C：Hello World
来源：http://hz.cqqwz.cn/gtggtpokls.html

#include <stdio.h>
来源：http://hz.shanyushiyangtech.top/gtgfsfygle.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.daria6918.cn/gtygueuvne.html

[S02] C：变量与格式化输出
来源：http://hz.daxiang520.top/gtlwkqfltg.html

int a = 10; printf("%d\n", a);
来源：http://hz.ybcxt.top/gtesninxbc.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtrjsbvymh.html

int x; scanf("%d", &x);
来源：http://hz.jinghuilouyu.cn/gtfwzttfny.html

[S04] C：字符串复制
来源：http://hz.sweek.top/gtwqrjttll.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtxkojiqkb.html

[S05] C：字符串长度
来源：http://hz.wangshuangyany.cn/gtbukcaxay.html

strlen(s)
来源：http://hz.redwolf501.top/gttyngdznt.html

[S06] C：字符串比较
来源：http://hz.jlsjyb.cn/gthfxfnrce.html

strcmp(a, b) == 0
来源：http://hz.shzxlz.cn/gtvufsntik.html

[S07] C：数组遍历求和
来源：http://hz.chenzaomai.com/gttneeywir.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtryqbyugg.html

[S08] C：动态内存分配与释放
来源：http://hz.fengsongda.top/gtkeaxwwyy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigufen.top/gtitndwezr.html

[S09] C：结构体定义与初始化
来源：http://hz.fzhhl.top/gtfjsvkzga.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tanke756.top/gtgsrlvauw.html

[S10] C：指针与解引用
来源：http://hz.dashuyun.cn/gtuetjepvr.html

int *p = &a;  *p = 5;
来源：http://hz.jlsjyb.cn/gtkhgbbhkw.html

[S11] C：逐行读文件
来源：http://hz.guannengcc.top/gtsavhmuwa.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cucudq.cn/gtipplewem.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.sxryk.cn/gtyqbzcjec.html

fclose(f);
来源：http://hz.shuidangran.top/gtdezkkfha.html

[S12] C：写文件
来源：http://hz.yj20258.top/gtodbewbrh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtbybgynyw.html

[S13] C：宏定义
来源：http://hz.yuxming.cn/gtkndhvmjc.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shzxlz.cn/gtaeiakrvu.html

[S14] C：枚举
来源：http://hz.9152youxi.cn/gteymasxni.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.aizwys.cn/gtvmyxoeia.html

[S15] C：类型转换
来源：http://hz.shuidangran.top/gtaglcofhd.html

(double) a / b
来源：http://hz.gaohongyu789.top/gtvmdxslhj.html

[S16] C：位操作置位
来源：http://hz.jianghu66.top/gtccuikotq.html

x |= (1 << 3);
来源：http://hz.xinyue.icu/gtqqacwqux.html

[S17] C：安全拼接字符串
来源：http://hz.jinqigfzy.top/gthhjbqaje.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shuidangran.top/gtgxqjxktr.html

[S18] C：命令行参数
来源：http://hz.tanke756.top/gtflzbuyyr.html

int main(int argc, char **argv)
来源：http://hz.xziqi.cn/gtyqgfltaw.html

[S19] C：快速排序
来源：http://hz.nanxuanxn.top/gtfmwcnijb.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cdnleiting.top/gtzypwctdw.html

[S20] C：二分查找
来源：http://hz.chenzaomai.com/gtkipozngj.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ydzc1.top/gtydzvvkkm.html

[S21] C：字符类别判断
来源：http://hz.cdnleiting.top/gtqqhmklds.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ydjk.org.cn/gtmypavsrj.html

[S22] C：字符串转数字
来源：http://hz.cheryme.top/gtoungouiy.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.guowangkeji.top/gtiywivwjv.html

[S23] C：随机数
来源：http://hz.316326.xyz/gtdjqakasc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.iojbl.cn/gtemtjxpti.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangtech.top/gtrfbcnwpd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.nwbrower.top/gtnuwlajwq.html

[S25] C：内存拷贝
来源：http://hz.svipenyu.cn/gtrpkeyhal.html

memcpy(dst, src, n);
来源：http://hz.zhaomingkeji.xyz/gthfpamvoo.html

[S26] C：内存清零
来源：http://hz.haohaochexian.top/gtjropvmic.html

memset(a, 0, sizeof a);
来源：http://hz.jlsjyb.cn/gtmodlskhq.html

[S27] C：定义常量
来源：http://hz.birdmap.top/gtibwygwcd.html

const double PI = 3.14159;
来源：http://hz.yj20258888.top/gtrjbrlzmq.html

[S28] C：静态变量
来源：http://hz.wangshuangyany.cn/gtowkistrc.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtitbmdkbg.html

[S29] C：变参函数
来源：http://hz.shangyingyoupin.top/gtjpaviggh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxuanxn.top/gtrtagqwfs.html

[S30] C：头文件保护
来源：http://hz.cqqwz.cn/gtrenejkxf.html

#ifndef X_H
来源：http://hz.tanke756.top/gtipjzqvtl.html

#define X_H
来源：http://hz.zycfv.cn/gtiappujpu.html

#endif
来源：http://hz.andypj.xyz/gtoreqijol.html

[S31] C++：Hello World
来源：http://hz.zdqjudy.top/gtolyhpljc.html

#include <iostream>
来源：http://hz.wangshuangyany.cn/gtayzzrgkt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yj202588.top/gtllcjcxju.html

[S32] C++：字符串
来源：http://hz.0kj1m.cn/gtdxdqpyhn.html

std::string s = "hi";  s += "!";
来源：http://hz.ivvv.top/gteutalufr.html

[S33] C++：vector 增删
来源：http://hz.yj20258888.top/gtbpwzzmfe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.mhx1999.top/gtnsfptrpi.html

[S34] C++：遍历 vector
来源：http://hz.zhongyouzk.top/gtstuyucwb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.daxiang520.top/gtgxrtvvob.html

[S35] C++：map
来源：http://hz.tanke756.top/gttfzupglm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuanzhike.top/gtfhqdfrvj.html

[S36] C++：unordered_map
来源：http://hz.zhengqikj.top/gtpzticmgx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yj202588.top/gthttqaqqi.html

[S37] C++：set
来源：http://hz.yueranfly.top/gtgqtspbra.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtqvnwinpd.html

[S38] C++：排序
来源：http://hz.chenzaomai.com/gtvxfjhnvz.html

std::sort(v.begin(), v.end());
来源：http://hz.zhaomingkeji.xyz/gtssbdrnsz.html

[S39] C++：自定义比较器排序
来源：http://hz.zhiwuduotai.top/gtdxhgwpdb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhiwuduotai.top/gtijbetdgo.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtbpgiebzl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yonumen.top/gtqmasydvz.html

[S41] C++：类与构造函数
来源：http://hz.cashguo.top/gtdktvkzjs.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ywan-chungtsiang.top/gtwfqnytis.html

[S42] C++：继承与虚函数
来源：http://hz.shuidangran.top/gthuevbeph.html

class B : public Base { public: void f() override {} };
来源：http://hz.316326.xyz/gtlxblstzl.html

[S43] C++：智能指针
来源：http://hz.xuanzx.com/gttbndfsui.html

auto p = std::make_unique<int>(5);
来源：http://hz.hnxiangtu.top/gtvvwchtoh.html

[S44] C++：引用传参
来源：http://hz.cucudq.cn/gtjhkayniv.html

void inc(int &x) { ++x; }
来源：http://hz.zhoulong.xyz/gtsxkhtvkl.html

[S45] C++：lambda
来源：http://hz.pycfn.com/gthbvcoqsy.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.tianlin.xyz/gtlelhriqy.html

[S46] C++：函数模板
来源：http://hz.jinyuanbaomall.cn/gtlfvzuxrz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.nanxinkj.top/gthizzrqwi.html

[S47] C++：结构化绑定遍历
来源：http://hz.gaohongyu789.top/gtdtulpbla.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.jlsjyb.cn/gthluuldib.html

[S48] C++：逐行读文件
来源：http://hz.yongpay.top/gtcuzkywel.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.hammf.cn/gtkukdswqf.html

while (std::getline(in, line)) { }
来源：http://hz.52xcode.cn/gtmswgbhnk.html

[S49] C++：写文件
来源：http://hz.tian-w.cn/gtatxbfzmn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.haohaochexian.top/gtkfcfiobl.html

[S50] C++：格式化数字
来源：http://hz.shzxlz.cn/gtocuogqmf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.pengpengdd.cyou/gtotaulrmw.html

[S51] C++：显式类型转换
来源：http://hz.cdnleiting.top/gtgxfpixpv.html

static_cast<double>(a) / b
来源：http://hz.wangdashe.top/gtjkhfxaqe.html

[S52] C++：const 与 noexcept
来源：http://hz.aibaodan.cn/gtfofllctk.html

int size() const noexcept { return n_; }
来源：http://hz.ydjk.org.cn/gtnpkpbspc.html

[S53] C++：移动语义
来源：http://hz.jinyuanbaomall.cn/gtdnlkcoup.html

std::vector<int> w = std::move(v);
来源：http://hz.fengsongda.top/gtplfqxorf.html

[S54] C++：异常处理
来源：http://hz.xingfuxueyuan.xyz/gtpoladopm.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtculfvudo.html

[S55] C++：结构化绑定
来源：http://hz.mhx1999.top/gtlbuwvkvm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.yj202588.top/gtmumpwlqu.html

[S56] C++：optional
来源：http://hz.cucudq.cn/gtjhszuxzn.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fzhhl.top/gtnybxijwr.html

[S57] C++：编译期常量
来源：http://hz.nanxinkj.top/gtralkszrb.html

constexpr int N = 10;
来源：http://hz.shzxlz.cn/gtdjsbjnul.html

[S58] C++：命名空间
来源：http://hz.guannengcc.top/gtvuxryndo.html

namespace ns { int f() { return 1; } }
来源：http://hz.bjfxy.top/gtzlaeoeka.html

[S59] C++：静态断言
来源：http://hz.zhaomingkeji.xyz/gtoqilfjzm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.smart0.xyz/gtzjijcijo.html

[S60] C++：遍历并删除元素
来源：http://hz.tianlin.xyz/gtxvqcdsvv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.chenjidiqi.icu/gtarqwkltp.html

================================================================================
来源：http://hz.xinyue.icu/gtdefkytzq.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.zhongyouzk.top/gthgptmdfu.html

================================================================================
来源：http://hz.cqqwz.cn/gtnebzjiga.html

[T01] Kotlin：Hello World
来源：http://hz.hywenlv.cn/gtkqkuhkyd.html

println("Hello")
来源：http://hz.ydzc1.top/gtthehkfbe.html

[T02] Kotlin：变量
来源：http://hz.sxryk.cn/gttkaaxqsr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.zhongyouzk.top/gtqrqayhkh.html

[T03] Kotlin：字符串模板
来源：http://hz.zdqjudy.top/gtzuupyemj.html

"值: $b"
来源：http://hz.zhaomingkeji.xyz/gtsastusri.html

[T04] Kotlin：空安全
来源：http://hz.quarkkingdee.top/gtrgxriaxz.html

val n: String? = null;  n?.length
来源：http://hz.jlsjyb.cn/gtuwkrclta.html

[T05] Kotlin：when 表达式
来源：http://hz.xinyue.icu/gtyocvmqbm.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.daria6918.cn/gtslaieddm.html

[T06] Kotlin：集合映射
来源：http://hz.yvedp.cn/gtplqwmflt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhoulong.xyz/gtbsspmpfc.html

[T07] Kotlin：集合过滤
来源：http://hz.hnqzz.top/gtrbonfcqv.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.bjfxy.top/gtliibgbno.html

[T08] Kotlin：数据类
来源：http://hz.guannengcc.top/gtowfvctjo.html

data class User(val name: String, val age: Int)
来源：http://hz.yuanzhike.top/gtcoodhklg.html

[T09] Kotlin：扩展函数
来源：http://hz.gaohongyu789.top/gthakrknoh.html

fun String.exclaim() = this + "!"
来源：http://hz.shzxlz.cn/gtwoothgcw.html

[T10] Kotlin：默认参数
来源：http://hz.hongshengwenyu.top/gtfhladtmd.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.hnqzz.top/gtyldxwpjr.html


<!-- 参考信息 -->