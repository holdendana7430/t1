代发 wailian999

case "$1" in
来源：http://hz.sweek.top/gtbodrngye.html

start) echo "启动" ;;
来源：http://hz.chenlongwang.top/gtpukqahnu.html

stop)  echo "停止" ;;
来源：http://hz.cdnleiting.top/gtecleugwi.html

*)     echo "未知命令" ;;
来源：http://hz.yuxming.cn/gtkiuxefvg.html

esac
来源：http://hz.meibo888.top/gteokqvewo.html

[R12] for 遍历文件
来源：http://hz.cheryme.top/gtggffalir.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhijiandao.cn/gtqyiohvlq.html

[R13] for 计数循环
来源：http://hz.yangfankeji.com/gtifyldahb.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.xylfe.cn/gtooihrhfa.html

[R14] C 风格 for
来源：http://hz.birdmap.top/gtyfkptyxl.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.fengsongda.top/gtzxckkqrs.html

[R15] while 逐行读文件
来源：http://hz.cashguo.top/gthrcemvuv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.nwbrower.top/gtxkstvqth.html

[R16] until 等待条件
来源：http://hz.zhixingplan.top/gtmipjomzt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gotoacloud.top/gtxednwqct.html

[R17] 数组定义与取值
来源：http://hz.0kj1m.cn/gtmrickgyc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinyuanbaomall.cn/gtopuzrsdk.html

[R18] 遍历数组
来源：http://hz.xingfuxueyuan.xyz/gtkvpbzfee.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xuanzx.com/gtrndfotrv.html

[R19] 数组长度
来源：http://hz.wangshuangyany.cn/gtcrqheoqf.html

echo "${#arr[@]}"
来源：http://hz.quarkkingdee.top/gtqnegtvav.html

[R20] 关联数组（字典）
来源：http://hz.aibaodan.cn/gtmtotjgse.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.xylfe.cn/gtygpefnbv.html

[R21] 字符串长度
来源：http://hz.shzxlz.cn/gtxzerecgu.html

echo "${#s}"
来源：http://hz.daria6918.cn/gtrcsipccu.html

[R22] 截取子串
来源：http://hz.cucudq.cn/gtcgyrgrep.html

echo "${s:0:5}"
来源：http://hz.tianlin.xyz/gtivcdkqhs.html

[R23] 字符串替换
来源：http://hz.feifeiyinyue.top/gtiosdbkjm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.hnqzz.top/gtbkcvwxel.html

[R24] 大小写转换
来源：http://hz.ppjwa.cn/gtumumnqjd.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnqzz.top/gtttlrmtwa.html

[R25] 去后缀 / 去前缀
来源：http://hz.hysaishi.cn/gtacpzamns.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.redwolf501.top/gtanhdlzzm.html

[R26] 命令替换
来源：http://hz.gogol.net.cn/gtnllyziys.html

now=$(date +%F); echo "$now"
来源：http://hz.yj202588.top/gtikrlmwdt.html

[R27] 算术展开
来源：http://hz.xingfuxueyuan.xyz/gtlixblvqk.html

echo $((1 + 2 * 3))
来源：http://hz.xylfe.cn/gtrsqgfmqo.html

[R28] 浮点运算
来源：http://hz.vqdsnc.cn/gtywusqvrn.html

echo "scale=2; 10/3" | bc
来源：http://hz.zhiwuduotai.top/gtleftyrhw.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtadmktvpb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.mhx1999.top/gtmncphupo.html

[R30] 函数返回状态码
来源：http://hz.hnqzz.top/gtjgohlxqr.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zhaomingkeji.xyz/gtldgdmubu.html

[R31] 局部变量
来源：http://hz.zhoulong.xyz/gttpovbdcg.html

f() { local x=1; echo "$x"; }
来源：http://hz.fengsongda.top/gtvsxfbexx.html

[R32] 参数个数校验
来源：http://hz.yj202588.top/gtgqfsodol.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtytqdrfyv.html

[R33] 捕获错误并提示行号
来源：http://hz.zdqjudy.top/gtvgugknug.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.sxryk.cn/gttudxtipe.html

[R34] 退出时清理
来源：http://hz.hywenlv.cn/gtwzsefyie.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtiahhvkxm.html

[R35] 后台执行并等待
来源：http://hz.tian-w.cn/gthwepifee.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.kuanghao11.cn/gtvnymmxzx.html

[R36] 并发执行多个任务
来源：http://hz.hammf.cn/gtfnthxlfb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.aibaodan.cn/gthgwzfvnl.html

[R37] 把输出赋给变量
来源：http://hz.sxryk.cn/gtohmhyzxj.html

files=$(ls -1)
来源：http://hz.aibaodan.cn/gtatpwsqrc.html

[R38] 管道串联
来源：http://hz.svipenyu.cn/gtfznwkggw.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yangfankeji.com/gtknkuxquk.html

[R39] 重定向标准输出与错误
来源：http://hz.yuanzhike.top/gtsbqyecyi.html

cmd > out.log 2>&1
来源：http://hz.meibo888.top/gtiuvhvdbg.html

[R40] 追加写日志
来源：http://hz.zhiwuduotai.top/gtsxuiuvds.html

echo "log" >> out.log
来源：http://hz.bjfxy.top/gtbgvgwcqz.html

[R41] 丢弃输出
来源：http://hz.yj202588.top/gtuqoxjhuc.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtxrnlhpux.html

[R42] 输入重定向
来源：http://hz.pycfn.com/gtutfemodo.html

wc -l < a.txt
来源：http://hz.ywan-chungtsiang.top/gtamavlgcw.html

[R43] 按名字查找文件
来源：http://hz.yuanzhike.top/gtweeakrdm.html

find . -name "*.log" -type f
来源：http://hz.nwbrower.top/gtlosrkiul.html

[R44] 按修改时间查找
来源：http://hz.redwolf501.top/gttizighkv.html

find . -mtime -7 -type f
来源：http://hz.zhiwuduotai.top/gttbvjjiaf.html

[R45] 批量删除
来源：http://hz.jqgufenzy.top/gtmipfdetd.html

find . -name "*.tmp" -delete
来源：http://hz.xuetiantiany.cn/gtowtnrypu.html

[R46] 递归替换文件内容
来源：http://hz.jqgfzy.top/gtbhjxtfbb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.zdqjudy.top/gtqmjbotnf.html

[R47] sed 单行替换
来源：http://hz.ppjwa.cn/gtehkowsed.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.xinyue.icu/gtzzolough.html

[R48] awk 取指定列
来源：http://hz.yangfankeji.com/gtgjqilcyw.html

awk '{print $1, $3}' a.txt
来源：http://hz.shanyushiyangkeji.top/gttghjuzjg.html

[R49] awk 带条件
来源：http://hz.dianchejie.cn/gtekkqkoae.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.kuanghao11.cn/gttzjrjpac.html

[R50] awk 求和
来源：http://hz.fengsongda.top/gtjnpchhmw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.feifeiyinyue.top/gtevltxryx.html

[R51] 排序去重取前几
来源：http://hz.xylfe.cn/gtmpzklfzv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.jianghu66.top/gttbhbbkkf.html

[R52] 统计行数
来源：http://hz.jinqigfzy.top/gtbhkspolx.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gttwqkwmuh.html

[R53] 查看文件头与实时尾
来源：http://hz.dianchejie.cn/gtzptbjozp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ybcxt.top/gtxpbyvyud.html

[R54] 比较两个文件
来源：http://hz.gogol.net.cn/gtgeynafps.html

diff a.txt b.txt
来源：http://hz.jqgufenzy.top/gtbicdsmau.html

[R55] 压缩与解压
来源：http://hz.jiagoushi.top/gtytbksqyp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.c1oappe.top/gtjjxxlfyd.html

[R56] 远程拷贝
来源：http://hz.redwolf501.top/gtwpupgjnl.html

scp file user@host:/path/
来源：http://hz.kuanghao11.cn/gtciinvinc.html

[R57] 远程执行命令
来源：http://hz.aibaodan.cn/gtmkqpjyyx.html

ssh user@host 'uptime'
来源：http://hz.havefunace.top/gtxvdfrlte.html

[R58] 下载文件
来源：http://hz.tian-w.cn/gtscmqqxmj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtrcqgnsfb.html

[R59] 发 POST JSON
来源：http://hz.jlsjyb.cn/gtuhzjngbo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.redwolf501.top/gtapzeyuep.html

[R60] 只看 HTTP 状态码
来源：http://hz.xuetiantiany.cn/gtjyqbwkke.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.redwolf501.top/gtoywgzafj.html

[R61] 磁盘占用
来源：http://hz.yj202588.top/gttvhuxtob.html

df -h;  du -sh *
来源：http://hz.hysaishi.cn/gtgefwovcb.html

[R62] 找最占空间的文件
来源：http://hz.cqqwz.cn/gtkezsklsl.html

du -ah . | sort -rh | head -10
来源：http://hz.316326.xyz/gtbejzpikj.html

[R63] 内存与进程
来源：http://hz.zhijiandao.cn/gtvvvifxlh.html

free -h;  ps aux | grep nginx
来源：http://hz.xingfuxueyuan.xyz/gtaapluuit.html

[R64] 结束进程
来源：http://hz.xuetiantiany.cn/gtjnrekuyi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.quarkkingdee.top/gtymbgprhr.html

[R65] 查看端口占用
来源：http://hz.shuidangran.top/gtgenfgnpm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.quarkkingdee.top/gtqcsfkmyu.html

[R66] 定时任务
来源：http://hz.aizwys.cn/gtwshhtzqu.html

crontab -e;  crontab -l
来源：http://hz.316326.xyz/gththqnchs.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtthcybepm.html

openssl rand -hex 16
来源：http://hz.andypj.xyz/gtrdivdvbp.html

[R68] 计算文件校验值
来源：http://hz.gotoacloud.top/gtpuuxluwv.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.c1oappe.top/gtfhspinkf.html

[R69] 生成随机密码
来源：http://hz.zhixingplan.top/gtrgummnig.html

head -c 16 /dev/urandom | base64
来源：http://hz.cashguo.top/gtemjoreba.html

[R70] 时间戳与互转
来源：http://hz.pengpengdd.cyou/gttmyvobxm.html

date +%s;  date -d @1700000000
来源：http://hz.nanxinkj.top/gtgtvdyuey.html

[R71] 日期格式化
来源：http://hz.zdqjudy.top/gtiuqgtfqu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.guannengcc.top/gtozktctav.html

[R72] 等待端口就绪
来源：http://hz.shanyushiyangkeji.top/gtnysphmol.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtqsdaqjsv.html

[R73] 分割大日志
来源：http://hz.iojbl.cn/gtgcchasnd.html

split -l 1000 big.log part_
来源：http://hz.hysaishi.cn/gtajmxfgqw.html

[R74] 批量重命名
来源：http://hz.tianlin.xyz/gtucdzisci.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hongshengwenyu.top/gthzupaayg.html

[R75] 导出环境变量
来源：http://hz.vqdsnc.cn/gtcfnksavx.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.ppjwa.cn/gtmjjbrcie.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtlcjwoslf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.dianchejie.cn/gtsqtktnql.html

[R77] 读取用户输入
来源：http://hz.vqdsnc.cn/gtrvcvzxdb.html

read -rp "请输入: " ans
来源：http://hz.redwolf501.top/gtilgtnpah.html

[R78] 交互式菜单
来源：http://hz.ehwqpu.com/gtpjucfezc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.sweek.top/gteppyndqj.html

[R79] 解析命令行选项
来源：http://hz.pycfn.com/gtgmnvopag.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ehwqpu.com/gtlyiddmbx.html

[R80] 查看脚本执行耗时
来源：http://hz.nanxuanxn.top/gtajsrzvws.html

time ./run.sh
来源：http://hz.c1oappe.top/gtjaivnkdv.html

================================================================================
来源：http://hz.cheryme.top/gtunvllgur.html

S. C / C++ 专题
来源：http://hz.meibo888.top/gtftrpuvin.html

================================================================================
来源：http://hz.9152youxi.cn/gtubolwbci.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtpgpkhjkw.html

#include <stdio.h>
来源：http://hz.yueranfly.top/gtfqrlepgp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gtytcswycj.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtasakthow.html

int a = 10; printf("%d\n", a);
来源：http://hz.smart0.xyz/gtbgcroxdl.html

[S03] C：读入整数
来源：http://hz.gogol.net.cn/gtdihnhsaz.html

int x; scanf("%d", &x);
来源：http://hz.andypj.xyz/gtihaksqgy.html

[S04] C：字符串复制
来源：http://hz.yangfankeji.com/gtrosnunss.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.shzxlz.cn/gtzowvrorc.html

[S05] C：字符串长度
来源：http://hz.yangfankeji.com/gtvgpoqasc.html

strlen(s)
来源：http://hz.yonumen.top/gtqgbfxnmf.html

[S06] C：字符串比较
来源：http://hz.sufxvd.cn/gtnyuinouc.html

strcmp(a, b) == 0
来源：http://hz.sysykeji.top/gtwnzaghzi.html

[S07] C：数组遍历求和
来源：http://hz.ybcxt.top/gtlvjgdcuy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.hysaishi.cn/gtajhsjabt.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtltapsbvl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.cheryme.top/gtjcxtloma.html

[S09] C：结构体定义与初始化
来源：http://hz.jqgufenzy.top/gtssoogyhi.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxinkj.top/gtqldvjyqr.html

[S10] C：指针与解引用
来源：http://hz.shuidangran.top/gtcsmipxvo.html

int *p = &a;  *p = 5;
来源：http://hz.jqgufenzy.top/gtntxwjaxb.html

[S11] C：逐行读文件
来源：http://hz.sxryk.cn/gtktgcimkv.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.gzhubu.top/gttlwtnajt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtnfavyjnp.html

fclose(f);
来源：http://hz.pycfn.com/gtyzctkjmu.html

[S12] C：写文件
来源：http://hz.jyoumei.cn/gtzvjhoxen.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.cashguo.top/gtceruznuk.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtcgdwjfnw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.gzhubu.top/gtxxzsirsd.html

[S14] C：枚举
来源：http://hz.tian-w.cn/gtspghdoje.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.gogol.net.cn/gtpernrmqr.html

[S15] C：类型转换
来源：http://hz.ybcxt.top/gtfgjfamzy.html

(double) a / b
来源：http://hz.shangyingyoupin.top/gtyleftrvj.html

[S16] C：位操作置位
来源：http://hz.jqgfzy.top/gtpaomvyjq.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtpjxtqlru.html

[S17] C：安全拼接字符串
来源：http://hz.yanxiufei.cn/gttezdlkgo.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.sufxvd.cn/gtuitsmjro.html

[S18] C：命令行参数
来源：http://hz.fengsongda.top/gtydygovhn.html

int main(int argc, char **argv)
来源：http://hz.wangdashe.top/gtqovcmepv.html

[S19] C：快速排序
来源：http://hz.hongshengwenyu.top/gtgenixibc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtkokpguja.html

[S20] C：二分查找
来源：http://hz.jinqigufen.top/gtchdhwtuf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yj20258.top/gtlvfqzozj.html

[S21] C：字符类别判断
来源：http://hz.jinghuilouyu.cn/gtlqjxyzas.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ivvv.top/gteuabgict.html

[S22] C：字符串转数字
来源：http://hz.jinghuilouyu.cn/gtrdwkodgi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.smart0.xyz/gtpuylmtnz.html

[S23] C：随机数
来源：http://hz.gogol.net.cn/gtkbhbzlbd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.vqdsnc.cn/gttvzzroyi.html

[S24] C：获取本地时间
来源：http://hz.jianghu66.top/gtqvdxxznm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.quarkkingdee.top/gtkkhioeql.html

[S25] C：内存拷贝
来源：http://hz.xziqi.cn/gtfvgktqlo.html

memcpy(dst, src, n);
来源：http://hz.ppjwa.cn/gtcocbyvsl.html

[S26] C：内存清零
来源：http://hz.yj20258.top/gtcuwzvosf.html

memset(a, 0, sizeof a);
来源：http://hz.gaohongyu789.top/gtwvohrqsx.html

[S27] C：定义常量
来源：http://hz.bjfxy.top/gtkkyskzbn.html

const double PI = 3.14159;
来源：http://hz.kuanghao11.cn/gtvvziwoaw.html

[S28] C：静态变量
来源：http://hz.jyoumei.cn/gtsoberzqu.html

static int counter = 0;
来源：http://hz.birdmap.top/gtazzyhdgx.html

[S29] C：变参函数
来源：http://hz.guannengcc.top/gtcnfsddae.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.daria6918.cn/gtsnymbvto.html

[S30] C：头文件保护
来源：http://hz.bjfxy.top/gtpvdipcuk.html

#ifndef X_H
来源：http://hz.jyoumei.cn/gtfdinkscx.html

#define X_H
来源：http://hz.guannengcc.top/gtojlkvizj.html

#endif
来源：http://hz.yuanzhike.top/gtdheiraoi.html

[S31] C++：Hello World
来源：http://hz.ppjwa.cn/gtddjlmuyc.html

#include <iostream>
来源：http://hz.pengpengdd.cyou/gtgjckmokw.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.svipenyu.cn/gtnvcfqadk.html

[S32] C++：字符串
来源：http://hz.sxryk.cn/gtzhnqbmud.html

std::string s = "hi";  s += "!";
来源：http://hz.zhaomingkeji.xyz/gtsunuyhmb.html

[S33] C++：vector 增删
来源：http://hz.yanxiufei.cn/gteofzmbyy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.smart0.xyz/gtowbdxfmv.html

[S34] C++：遍历 vector
来源：http://hz.zhiwuduotai.top/gtltpbcdbt.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.dianchejie.cn/gtknynjbef.html

[S35] C++：map
来源：http://hz.vqdsnc.cn/gtqejaiuty.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.hongshengwenyu.top/gtztegcjlr.html

[S36] C++：unordered_map
来源：http://hz.ywan-chungtsiang.top/gtktgfdjbh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gzhubu.top/gtdukjgkcu.html

[S37] C++：set
来源：http://hz.aizwys.cn/gtikoeifwa.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.316326.xyz/gtxlivakvj.html

[S38] C++：排序
来源：http://hz.xuanzx.com/gtxboxjwpk.html

std::sort(v.begin(), v.end());
来源：http://hz.zhoulong.xyz/gtvtfhhzzk.html

[S39] C++：自定义比较器排序
来源：http://hz.hongshengwenyu.top/gttpcqzzco.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.c1oappe.top/gtlieeabzi.html

[S40] C++：查找元素
来源：http://hz.jiagoushi.top/gtsohlducg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.jiagoushi.top/gtibcnlqhh.html

[S41] C++：类与构造函数
来源：http://hz.kuanghao11.cn/gtiiaupcti.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.xingfuxueyuan.xyz/gtnsvkvygn.html

[S42] C++：继承与虚函数
来源：http://hz.dashuyun.cn/gtwzuyvlyn.html

class B : public Base { public: void f() override {} };
来源：http://hz.jiagoushi.top/gtthmoqnvx.html

[S43] C++：智能指针
来源：http://hz.fengsongda.top/gtsczskers.html

auto p = std::make_unique<int>(5);
来源：http://hz.yueranfly.top/gtzostxlpk.html

[S44] C++：引用传参
来源：http://hz.mhx1999.top/gtlohdzgtk.html

void inc(int &x) { ++x; }
来源：http://hz.zhongyouzk.top/gteinmqeqi.html

[S45] C++：lambda
来源：http://hz.aizwys.cn/gtxhirwpgk.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.chenjidiqi.icu/gtpdxwazta.html

[S46] C++：函数模板
来源：http://hz.quarkkingdee.top/gtcpblkbeh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.fengsongda.top/gtjykdpgld.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj202588.top/gtlwxnqude.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.quarkkingdee.top/gttcfjhqxu.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtjivxdqkt.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.wangdashe.top/gtuwgbezmt.html

while (std::getline(in, line)) { }
来源：http://hz.guannengcc.top/gtjzwproyl.html

[S49] C++：写文件
来源：http://hz.hfpthk.cn/gtozscsyqn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.sweek.top/gtgvypipzi.html

[S50] C++：格式化数字
来源：http://hz.chenzaomai.com/gtveihceqh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.zhaomingkeji.xyz/gtkkmiffiz.html

[S51] C++：显式类型转换
来源：http://hz.jinyuanbaomall.cn/gttrtjwxtc.html

static_cast<double>(a) / b
来源：http://hz.tian-w.cn/gtyiskwsqf.html

[S52] C++：const 与 noexcept
来源：http://hz.daxiang520.top/gtpnkvzdhg.html

int size() const noexcept { return n_; }
来源：http://hz.shangyingyoupin.top/gtoshczlbr.html

[S53] C++：移动语义
来源：http://hz.shzxlz.cn/gtvjtepbuy.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtbsrtjbxz.html

[S54] C++：异常处理
来源：http://hz.jinyuanbaomall.cn/gtpnpqwzfz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.ppjwa.cn/gtsrqwnfku.html

[S55] C++：结构化绑定
来源：http://hz.jqgfzy.top/gtvaghkwcp.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.pycfn.com/gtwfksrzqx.html

[S56] C++：optional
来源：http://hz.jyoumei.cn/gtaqzdttgk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.zhixingplan.top/gtelagusoh.html

[S57] C++：编译期常量
来源：http://hz.svipenyu.cn/gtveyeelmn.html

constexpr int N = 10;
来源：http://hz.sufxvd.cn/gtnsssoujl.html

[S58] C++：命名空间
来源：http://hz.gogol.net.cn/gtgmztkaze.html

namespace ns { int f() { return 1; } }
来源：http://hz.shanyushiyangtech.top/gttoezavcq.html

[S59] C++：静态断言
来源：http://hz.cucudq.cn/gtuxqrenmm.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.tianlin.xyz/gtsudnbfyw.html

[S60] C++：遍历并删除元素
来源：http://hz.redwolf501.top/gtuaysmjto.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.sufxvd.cn/gthujpfcgh.html

================================================================================
来源：http://hz.havefunace.top/gtevmebvwv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dashuyun.cn/gteetvrtvg.html

================================================================================
来源：http://hz.cheryme.top/gtgskndagm.html

[T01] Kotlin：Hello World
来源：http://hz.cashguo.top/gtkzmtnzty.html

println("Hello")
来源：http://hz.ivvv.top/gtmfeebqmt.html

[T02] Kotlin：变量
来源：http://hz.daxiang520.top/gtdjcxprew.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.wangshuangyany.cn/gtjwbcbauc.html

[T03] Kotlin：字符串模板
来源：http://hz.meibo888.top/gtcljnyojm.html

"值: $b"
来源：http://hz.birdmap.top/gtzkuigtzm.html

[T04] Kotlin：空安全
来源：http://hz.gotoacloud.top/gtvogneuit.html

val n: String? = null;  n?.length
来源：http://hz.aizwys.cn/gtzguewdvt.html

[T05] Kotlin：when 表达式
来源：http://hz.guowangkeji.top/gtdalcclwa.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.zhengqikj.top/gtjsmjxqmz.html

[T06] Kotlin：集合映射
来源：http://hz.9152youxi.cn/gtrlpodznl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.nanxuanxn.top/gtquhmrtsi.html

[T07] Kotlin：集合过滤
来源：http://hz.pycfn.com/gtqulebtzb.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.xziqi.cn/gtfcazdcvm.html

[T08] Kotlin：数据类
来源：http://hz.zhixingplan.top/gtyvmkkdkv.html

data class User(val name: String, val age: Int)
来源：http://hz.hammf.cn/gttwgehhuh.html

[T09] Kotlin：扩展函数
来源：http://hz.yongpay.top/gtwxanuovr.html

fun String.exclaim() = this + "!"
来源：http://hz.jiagoushi.top/gtenynnwou.html

[T10] Kotlin：默认参数
来源：http://hz.zhengqikj.top/gtmmpmdrsb.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.cheryme.top/gtlbndntbs.html

[T11] Kotlin：协程
来源：http://hz.jinyuanbaomall.cn/gtguvumyvc.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.yj20258888.top/gtcdbrgrdj.html

[T12] Kotlin：解构声明
来源：http://hz.snrcjt.cn/gtbyiennup.html

val (a, b) = Pair(1, 2)
来源：http://hz.jqgfzy.top/gtfyslzoop.html


<!-- 参考信息 -->