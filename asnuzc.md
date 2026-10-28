代发 wailian999

case "$1" in
来源：http://hz.havefunace.top/gtlvyubqpa.html

start) echo "启动" ;;
来源：http://hz.zhiwuduotai.top/gtgxpdbwzr.html

stop)  echo "停止" ;;
来源：http://hz.guowangkeji.top/gtoaxenuoj.html

*)     echo "未知命令" ;;
来源：http://hz.52xcode.cn/gtnqsdritg.html

esac
来源：http://hz.quarkkingdee.top/gtlzeoduhv.html

[R12] for 遍历文件
来源：http://hz.xinyue.icu/gtmegtbgft.html

for f in *.txt; do echo "$f"; done
来源：http://hz.jinqigfzy.top/gtbzxshlor.html

[R13] for 计数循环
来源：http://hz.xinyue.icu/gtqkxtcpjs.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.havefunace.top/gtpauvrwgu.html

[R14] C 风格 for
来源：http://hz.jqgufenzy.top/gtvwznrsfr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.9152youxi.cn/gtihtsvkah.html

[R15] while 逐行读文件
来源：http://hz.daria6918.cn/gtibgiagnu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.guowangkeji.top/gtqivuxufb.html

[R16] until 等待条件
来源：http://hz.birdmap.top/gtefrkjpvu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.xinyue.icu/gtxcwhiviy.html

[R17] 数组定义与取值
来源：http://hz.sysykeji.top/gtqextejuq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.chenjidiqi.icu/gtxvsyzskm.html

[R18] 遍历数组
来源：http://hz.yanxiufei.cn/gtabcjyrxe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.vqdsnc.cn/gtmbytsczk.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gttfaybzeb.html

echo "${#arr[@]}"
来源：http://hz.0kj1m.cn/gtogeofkny.html

[R20] 关联数组（字典）
来源：http://hz.haohaochexian.top/gtvquzgigp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zdqjudy.top/gthofdnari.html

[R21] 字符串长度
来源：http://hz.mhx1999.top/gtgalmhyhq.html

echo "${#s}"
来源：http://hz.mhx1999.top/gttrzfgbpp.html

[R22] 截取子串
来源：http://hz.xuanzx.com/gtjxfldjpi.html

echo "${s:0:5}"
来源：http://hz.gaohongyu789.top/gtjwaejhbe.html

[R23] 字符串替换
来源：http://hz.yj202588.top/gtpzvtpccs.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhixingplan.top/gtdykatkao.html

[R24] 大小写转换
来源：http://hz.jianghu66.top/gtesnwraka.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.daria6918.cn/gtxjpluaxo.html

[R25] 去后缀 / 去前缀
来源：http://hz.yj202588.top/gtuuenzpcx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.pycfn.com/gtabbffpyx.html

[R26] 命令替换
来源：http://hz.hammf.cn/gtbxxyclmt.html

now=$(date +%F); echo "$now"
来源：http://hz.zdqjudy.top/gtnuladfmk.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtvgqkkrxs.html

echo $((1 + 2 * 3))
来源：http://hz.ywan-chungtsiang.top/gtbxshywkv.html

[R28] 浮点运算
来源：http://hz.snrcjt.cn/gtmedascka.html

echo "scale=2; 10/3" | bc
来源：http://hz.fengsongda.top/gtgxmkuolt.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gttaznpabm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuetiantiany.cn/gtvivtfsvs.html

[R30] 函数返回状态码
来源：http://hz.xuetiantiany.cn/gtpkjpkqtc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.gaohongyu789.top/gtqeqjcita.html

[R31] 局部变量
来源：http://hz.ivvv.top/gtyxjgvjhv.html

f() { local x=1; echo "$x"; }
来源：http://hz.quarkkingdee.top/gteitdxffr.html

[R32] 参数个数校验
来源：http://hz.nwbrower.top/gtylvxfbiz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jinqigfzy.top/gtadflamkt.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtcynrcasp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.mhx1999.top/gtvwbitrcp.html

[R34] 退出时清理
来源：http://hz.ybcxt.top/gtxkwbkjhz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhijiandao.cn/gtxbpqipmb.html

[R35] 后台执行并等待
来源：http://hz.zdqjudy.top/gtgmapczup.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtwyqcxqdi.html

[R36] 并发执行多个任务
来源：http://hz.jinghuilouyu.cn/gtqxwumaif.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pengpengdd.cyou/gtzbcfttnr.html

[R37] 把输出赋给变量
来源：http://hz.wangdashe.top/gtldduadgh.html

files=$(ls -1)
来源：http://hz.fengsongda.top/gttfbtoemp.html

[R38] 管道串联
来源：http://hz.xuetiantiany.cn/gtjifgkdxc.html

cat a.txt | grep -i error | wc -l
来源：http://hz.feifeiyinyue.top/gtoxxvixfp.html

[R39] 重定向标准输出与错误
来源：http://hz.pengpengdd.cyou/gtrlijbmbv.html

cmd > out.log 2>&1
来源：http://hz.wangshuangyany.cn/gtefuwuewh.html

[R40] 追加写日志
来源：http://hz.tianlin.xyz/gtjihsnyfz.html

echo "log" >> out.log
来源：http://hz.xuanzx.com/gtsspcxpty.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtagqwsntw.html

cmd >/dev/null 2>&1
来源：http://hz.tanke756.top/gttrprtayq.html

[R42] 输入重定向
来源：http://hz.dashuyun.cn/gtsitnaaht.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtmhtunrum.html

[R43] 按名字查找文件
来源：http://hz.hfpthk.cn/gtxanyxzxb.html

find . -name "*.log" -type f
来源：http://hz.yj202588.top/gthnncnecc.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtkvjyoxvw.html

find . -mtime -7 -type f
来源：http://hz.sxryk.cn/gtfhhklxhf.html

[R45] 批量删除
来源：http://hz.mhx1999.top/gtyfiybsde.html

find . -name "*.tmp" -delete
来源：http://hz.aizwys.cn/gtpbgrtokd.html

[R46] 递归替换文件内容
来源：http://hz.hywenlv.cn/gthmjdbrff.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gaohongyu789.top/gttajaepcd.html

[R47] sed 单行替换
来源：http://hz.zhixingplan.top/gtbbwbnqxj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zhiwuduotai.top/gtotbsorpa.html

[R48] awk 取指定列
来源：http://hz.zhoulong.xyz/gtxgzsjqvu.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigufen.top/gtldczfdlt.html

[R49] awk 带条件
来源：http://hz.kuanghao11.cn/gtsjoqbdnb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhongyouzk.top/gtdsihdyqm.html

[R50] awk 求和
来源：http://hz.shangyingyoupin.top/gtrjvboxto.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtugdsgkor.html

[R51] 排序去重取前几
来源：http://hz.cheryme.top/gtmppkhqbu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ivvv.top/gtxapxgneq.html

[R52] 统计行数
来源：http://hz.hfpthk.cn/gtiykjmams.html

wc -l a.txt
来源：http://hz.ywan-chungtsiang.top/gtxbtzctqq.html

[R53] 查看文件头与实时尾
来源：http://hz.aibaodan.cn/gtdjzuumaa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daxiang520.top/gtuoirgoxn.html

[R54] 比较两个文件
来源：http://hz.kuanghao11.cn/gtjcvahuiy.html

diff a.txt b.txt
来源：http://hz.snrcjt.cn/gtwpaswjbq.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtegxqsxue.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.havefunace.top/gtjwsunolv.html

[R56] 远程拷贝
来源：http://hz.svipenyu.cn/gttrtlhewg.html

scp file user@host:/path/
来源：http://hz.hongshengwenyu.top/gteyftgycc.html

[R57] 远程执行命令
来源：http://hz.tian-w.cn/gtfpcjlmkd.html

ssh user@host 'uptime'
来源：http://hz.havefunace.top/gtdvcrjlaf.html

[R58] 下载文件
来源：http://hz.yj202588.top/gtxkhauywm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.aizwys.cn/gtcruhltso.html

[R59] 发 POST JSON
来源：http://hz.xziqi.cn/gtwoavqmvf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.kuanghao11.cn/gtjzjfihht.html

[R60] 只看 HTTP 状态码
来源：http://hz.vqdsnc.cn/gtpvkuidck.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.havefunace.top/gtkxiffyla.html

[R61] 磁盘占用
来源：http://hz.c1oappe.top/gtsevyckhu.html

df -h;  du -sh *
来源：http://hz.guowangkeji.top/gtglmejuzz.html

[R62] 找最占空间的文件
来源：http://hz.yj202588.top/gtpupftspj.html

du -ah . | sort -rh | head -10
来源：http://hz.daxiang520.top/gtpesknlps.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtqwiaxzmo.html

free -h;  ps aux | grep nginx
来源：http://hz.mhx1999.top/gtjbpimznb.html

[R64] 结束进程
来源：http://hz.zycfv.cn/gtcrqktcye.html

kill -9 $(pgrep -f app.py)
来源：http://hz.gaohongyu789.top/gtizollusk.html

[R65] 查看端口占用
来源：http://hz.shzxlz.cn/gtzgzeqfoj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.wangdashe.top/gtvjixbsgx.html

[R66] 定时任务
来源：http://hz.jqgfzy.top/gtjxcsyfba.html

crontab -e;  crontab -l
来源：http://hz.nanxuanxn.top/gtieohmgss.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtqnabrlug.html

openssl rand -hex 16
来源：http://hz.cheryme.top/gtaxthbxuj.html

[R68] 计算文件校验值
来源：http://hz.jqgfzy.top/gtagyptuke.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.xylfe.cn/gtbzpelyfn.html

[R69] 生成随机密码
来源：http://hz.havefunace.top/gtvcaebtjz.html

head -c 16 /dev/urandom | base64
来源：http://hz.hysaishi.cn/gtvumfsgmt.html

[R70] 时间戳与互转
来源：http://hz.dashuyun.cn/gtrlvpmryl.html

date +%s;  date -d @1700000000
来源：http://hz.ppjwa.cn/gtehbaxiwo.html

[R71] 日期格式化
来源：http://hz.chenlongwang.top/gtycjmnufh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.ydjk.org.cn/gtnwnqxnbl.html

[R72] 等待端口就绪
来源：http://hz.redwolf501.top/gtpuyawqth.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.jinyuanbaomall.cn/gthcljtqya.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gtzzywhgvv.html

split -l 1000 big.log part_
来源：http://hz.xziqi.cn/gtivlyqlav.html

[R74] 批量重命名
来源：http://hz.hnxiangtu.top/gtfxkgrqgj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.9152youxi.cn/gtmgcigtah.html

[R75] 导出环境变量
来源：http://hz.mhx1999.top/gtelqrwasn.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cheryme.top/gtewqewskr.html

[R76] 使用临时文件
来源：http://hz.hfpthk.cn/gthghmxayx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cheryme.top/gtupstjgld.html

[R77] 读取用户输入
来源：http://hz.xuetiantiany.cn/gtlvnogjcs.html

read -rp "请输入: " ans
来源：http://hz.hnqzz.top/gtfnpbfalc.html

[R78] 交互式菜单
来源：http://hz.jinghuilouyu.cn/gtjhklrvli.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.dashuyun.cn/gtkntvruuo.html

[R79] 解析命令行选项
来源：http://hz.iojbl.cn/gtjywykdag.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yongpay.top/gthhhpkvjy.html

[R80] 查看脚本执行耗时
来源：http://hz.tianlin.xyz/gtvpgsrphq.html

time ./run.sh
来源：http://hz.jianghu66.top/gtcadtrrcr.html

================================================================================
来源：http://hz.nanxinkj.top/gtnuqunkvw.html

S. C / C++ 专题
来源：http://hz.jianghu66.top/gtqsgdbsiv.html

================================================================================
来源：http://hz.c1oappe.top/gtwczqimde.html

[S01] C：Hello World
来源：http://hz.gaohongyu789.top/gtpigdjbzl.html

#include <stdio.h>
来源：http://hz.jiagoushi.top/gtfrdlqlva.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jqgufenzy.top/gtokayqgzb.html

[S02] C：变量与格式化输出
来源：http://hz.gogol.net.cn/gtocuhhkll.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtkynidvis.html

[S03] C：读入整数
来源：http://hz.zhixingplan.top/gtpbeaxeqz.html

int x; scanf("%d", &x);
来源：http://hz.chenlongwang.top/gtbsehjxtf.html

[S04] C：字符串复制
来源：http://hz.xuetiantiany.cn/gtmhhalfpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yvedp.cn/gtqcaojtuz.html

[S05] C：字符串长度
来源：http://hz.nwbrower.top/gtcdltstxa.html

strlen(s)
来源：http://hz.snrcjt.cn/gtpptiukih.html

[S06] C：字符串比较
来源：http://hz.snrcjt.cn/gtlmlvnlee.html

strcmp(a, b) == 0
来源：http://hz.yuxming.cn/gthzvozkyl.html

[S07] C：数组遍历求和
来源：http://hz.birdmap.top/gtnjknwbim.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.zhiwuduotai.top/gtalumhewe.html

[S08] C：动态内存分配与释放
来源：http://hz.smart0.xyz/gtsjcbwkxi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jianghu66.top/gtyqwcttqc.html

[S09] C：结构体定义与初始化
来源：http://hz.jinqigfzy.top/gtkswlljoj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.daxiang520.top/gtfjdgnmep.html

[S10] C：指针与解引用
来源：http://hz.cdnleiting.top/gtorbdpbnv.html

int *p = &a;  *p = 5;
来源：http://hz.hysaishi.cn/gtwnvrjucb.html

[S11] C：逐行读文件
来源：http://hz.316326.xyz/gtjeeufees.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.fzhhl.top/gtfhnsbvic.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.jyoumei.cn/gtkmqmnvwg.html

fclose(f);
来源：http://hz.nanxinkj.top/gtagafjxsj.html

[S12] C：写文件
来源：http://hz.jqgfzy.top/gtgqzquoqh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.0kj1m.cn/gtuygxfksn.html

[S13] C：宏定义
来源：http://hz.jqgfzy.top/gtgkprczho.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.9152youxi.cn/gtbsmzknvs.html

[S14] C：枚举
来源：http://hz.gogol.net.cn/gtanlkuxej.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cashguo.top/gtypviwecg.html

[S15] C：类型转换
来源：http://hz.zhaomingkeji.xyz/gtacrhxrcm.html

(double) a / b
来源：http://hz.zhongyouzk.top/gtljzlzxdp.html

[S16] C：位操作置位
来源：http://hz.zhongyouzk.top/gtsjloxmzd.html

x |= (1 << 3);
来源：http://hz.dianchejie.cn/gtkglgnznx.html

[S17] C：安全拼接字符串
来源：http://hz.hfpthk.cn/gtjqxnlpwa.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xuetiantiany.cn/gtgyhcpzgc.html

[S18] C：命令行参数
来源：http://hz.aizwys.cn/gtxtcceovz.html

int main(int argc, char **argv)
来源：http://hz.xziqi.cn/gtdacytvgv.html

[S19] C：快速排序
来源：http://hz.gaohongyu789.top/gtjuloguck.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.jianghu66.top/gtrydcolet.html

[S20] C：二分查找
来源：http://hz.ywan-chungtsiang.top/gtvkxivusu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtlfakfxhh.html

[S21] C：字符类别判断
来源：http://hz.gotoacloud.top/gtpnuekohg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.c1oappe.top/gtksthpdax.html

[S22] C：字符串转数字
来源：http://hz.gzhubu.top/gtchgwdcva.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.cucudq.cn/gttlmallei.html

[S23] C：随机数
来源：http://hz.c1oappe.top/gtfcbbtfqv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cucudq.cn/gtnxzkepkk.html

[S24] C：获取本地时间
来源：http://hz.xinyue.icu/gtxoecifbb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.chenjidiqi.icu/gtmvjjyakd.html

[S25] C：内存拷贝
来源：http://hz.jianghu66.top/gtvfhvtqyg.html

memcpy(dst, src, n);
来源：http://hz.zhixingplan.top/gtchftgqlz.html

[S26] C：内存清零
来源：http://hz.cqqwz.cn/gtrtmrnvcq.html

memset(a, 0, sizeof a);
来源：http://hz.ivvv.top/gtedlxeyab.html

[S27] C：定义常量
来源：http://hz.cheryme.top/gtvrvmaohi.html

const double PI = 3.14159;
来源：http://hz.wangdashe.top/gtopbgebcc.html

[S28] C：静态变量
来源：http://hz.smart0.xyz/gttpmikzhy.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtbojydlbe.html

[S29] C：变参函数
来源：http://hz.hywenlv.cn/gtuhtbwdxv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shuidangran.top/gtooartfxz.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtjtxnagjj.html

#ifndef X_H
来源：http://hz.jinqigufen.top/gtxiespvhm.html

#define X_H
来源：http://hz.yanxiufei.cn/gtepskulpt.html

#endif
来源：http://hz.hysaishi.cn/gtbngksslo.html

[S31] C++：Hello World
来源：http://hz.daxiang520.top/gtyfmjvshk.html

#include <iostream>
来源：http://hz.gzhubu.top/gtdfxahomd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yonumen.top/gtbzjccvig.html

[S32] C++：字符串
来源：http://hz.wangdashe.top/gtvndtshzt.html

std::string s = "hi";  s += "!";
来源：http://hz.daxiang520.top/gtnihvpqsb.html

[S33] C++：vector 增删
来源：http://hz.feifeiyinyue.top/gtsgkjociu.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hongshengwenyu.top/gtrfromtkb.html

[S34] C++：遍历 vector
来源：http://hz.yuxming.cn/gtjqzwihft.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ivvv.top/gtxnulcgwd.html

[S35] C++：map
来源：http://hz.ydzc1.top/gtuebzfizm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gtljkdamdk.html

[S36] C++：unordered_map
来源：http://hz.xinyue.icu/gtdfwmarcm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.zhoulong.xyz/gtwdzeiqcc.html

[S37] C++：set
来源：http://hz.havefunace.top/gtfspswpgm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.xziqi.cn/gtdttdcsau.html

[S38] C++：排序
来源：http://hz.fzhhl.top/gtnozbdqfc.html

std::sort(v.begin(), v.end());
来源：http://hz.xziqi.cn/gttuzwtwiq.html

[S39] C++：自定义比较器排序
来源：http://hz.tian-w.cn/gttaifkylr.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.bjfxy.top/gtgmgztdyw.html

[S40] C++：查找元素
来源：http://hz.wangshuangyany.cn/gtvwremteu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.sweek.top/gtkkzgsnrs.html

[S41] C++：类与构造函数
来源：http://hz.gogol.net.cn/gtwvoqziog.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.nanxinkj.top/gtluqsxhyd.html

[S42] C++：继承与虚函数
来源：http://hz.feifeiyinyue.top/gtvxbgvruf.html

class B : public Base { public: void f() override {} };
来源：http://hz.yj20258888.top/gtszmiljhj.html

[S43] C++：智能指针
来源：http://hz.havefunace.top/gtgbgywrhh.html

auto p = std::make_unique<int>(5);
来源：http://hz.gaohongyu789.top/gtueobzlah.html

[S44] C++：引用传参
来源：http://hz.birdmap.top/gtirkotiup.html

void inc(int &x) { ++x; }
来源：http://hz.meibo888.top/gthltitalx.html

[S45] C++：lambda
来源：http://hz.316326.xyz/gtthfvkbgl.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.nanxuanxn.top/gthnsuulza.html

[S46] C++：函数模板
来源：http://hz.snrcjt.cn/gtfvzpjcwv.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sufxvd.cn/gtrroofooi.html

[S47] C++：结构化绑定遍历
来源：http://hz.dianchejie.cn/gtbabycrhr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.tianlin.xyz/gtphdyhwtu.html

[S48] C++：逐行读文件
来源：http://hz.sxryk.cn/gtkgafcipo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.tian-w.cn/gtvielukop.html

while (std::getline(in, line)) { }
来源：http://hz.ehwqpu.com/gtsywzppfa.html

[S49] C++：写文件
来源：http://hz.52xcode.cn/gtjzhzfmig.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yonumen.top/gtpkkqujkc.html

[S50] C++：格式化数字
来源：http://hz.xziqi.cn/gtwvsubhuh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.aizwys.cn/gttrtfmtau.html

[S51] C++：显式类型转换
来源：http://hz.yj202588.top/gtfvofnngl.html

static_cast<double>(a) / b
来源：http://hz.cashguo.top/gtfrmtcmuy.html

[S52] C++：const 与 noexcept
来源：http://hz.yongpay.top/gttzwsocpx.html

int size() const noexcept { return n_; }
来源：http://hz.haohaochexian.top/gtzsxyreiw.html

[S53] C++：移动语义
来源：http://hz.haohaochexian.top/gtkrykfgfj.html

std::vector<int> w = std::move(v);
来源：http://hz.jinqigfzy.top/gtupqaixxv.html

[S54] C++：异常处理
来源：http://hz.chenzaomai.com/gtpbygkcmt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.kuanghao11.cn/gtqcigkved.html

[S55] C++：结构化绑定
来源：http://hz.jinyuanbaomall.cn/gtcmhbyvhz.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.tian-w.cn/gtoddnoprg.html

[S56] C++：optional
来源：http://hz.bjfxy.top/gtfyegsbma.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.jinyuanbaomall.cn/gtnktjikec.html

[S57] C++：编译期常量
来源：http://hz.andypj.xyz/gtwqvuhalg.html

constexpr int N = 10;
来源：http://hz.guowangkeji.top/gtzlikjmbq.html

[S58] C++：命名空间
来源：http://hz.hnqzz.top/gtkromltsd.html

namespace ns { int f() { return 1; } }
来源：http://hz.yj202588.top/gtwlypjidv.html

[S59] C++：静态断言
来源：http://hz.yuxming.cn/gtjkwwovha.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.hnqzz.top/gtxiauvaal.html

[S60] C++：遍历并删除元素
来源：http://hz.snrcjt.cn/gtssuqxeel.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.yuanzhike.top/gtkvdhcaef.html

================================================================================
来源：http://hz.hysaishi.cn/gtqgvcdaqe.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.guannengcc.top/gtsdqpaghw.html

================================================================================
来源：http://hz.chenlongwang.top/gttaahfltx.html

[T01] Kotlin：Hello World
来源：http://hz.kuanghao11.cn/gtkcdhqgwt.html

println("Hello")
来源：http://hz.tian-w.cn/gttdfakbyw.html

[T02] Kotlin：变量
来源：http://hz.nanxinkj.top/gtwvgmnspn.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.gzhubu.top/gtkqxjgspv.html

[T03] Kotlin：字符串模板
来源：http://hz.sysykeji.top/gtxztzhygc.html

"值: $b"
来源：http://hz.9152youxi.cn/gtjccgmjuh.html

[T04] Kotlin：空安全
来源：http://hz.chenjidiqi.icu/gtroizsqzj.html

val n: String? = null;  n?.length
来源：http://hz.chenlongwang.top/gtiqgdemca.html

[T05] Kotlin：when 表达式
来源：http://hz.zdqjudy.top/gtqrjkrbba.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.hfpthk.cn/gtldsnaoin.html

[T06] Kotlin：集合映射
来源：http://hz.shzxlz.cn/gtwjhmkokn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.zhijiandao.cn/gtzfnoemgf.html

[T07] Kotlin：集合过滤
来源：http://hz.xuanzx.com/gthbngiils.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.0kj1m.cn/gtijbgqfxt.html

[T08] Kotlin：数据类
来源：http://hz.ybcxt.top/gtpyavtpsg.html

data class User(val name: String, val age: Int)
来源：http://hz.nanxinkj.top/gtujucvlnf.html

[T09] Kotlin：扩展函数
来源：http://hz.yj20258.top/gtcztfcmxf.html

fun String.exclaim() = this + "!"
来源：http://hz.haohaochexian.top/gtsobuppaf.html

[T10] Kotlin：默认参数
来源：http://hz.gotoacloud.top/gtrcylzocx.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.aizwys.cn/gtficouhtj.html

[T11] Kotlin：协程
来源：http://hz.yuanzhike.top/gtejbfbtcw.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.daxiang520.top/gtirgnxlki.html

[T12] Kotlin：解构声明
来源：http://hz.yj20258888.top/gtfwiiatip.html

val (a, b) = Pair(1, 2)
来源：http://hz.ehwqpu.com/gtkdrgjowz.html


<!-- 参考信息 -->