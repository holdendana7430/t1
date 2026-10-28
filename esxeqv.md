代发 wailian999

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.cheryme.top/gtfkdbbfue.html

[R08] 数值比较
来源：http://hz.sxryk.cn/gtgusrdnss.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.gzhubu.top/gtzsukxmwh.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gtqiwfaoms.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.dianchejie.cn/gtybxnijuj.html

[R10] 正则匹配
来源：http://hz.yj202588.top/gteiexoboi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.cheryme.top/gtipqivptg.html

[R11] case 多分支
来源：http://hz.yj20258888.top/gtkxpwwzez.html

case "$1" in
来源：http://hz.fengsongda.top/gtqzmwgsav.html

start) echo "启动" ;;
来源：http://hz.shanyushiyangkeji.top/gthcruhjja.html

stop)  echo "停止" ;;
来源：http://hz.xinyue.icu/gtqnfxomqy.html

*)     echo "未知命令" ;;
来源：http://hz.jinghuilouyu.cn/gtnsgwdefp.html

esac
来源：http://hz.zhoulong.xyz/gthaztgneh.html

[R12] for 遍历文件
来源：http://hz.yonumen.top/gtllbmkaeb.html

for f in *.txt; do echo "$f"; done
来源：http://hz.gaohongyu789.top/gtyhvymqmb.html

[R13] for 计数循环
来源：http://hz.yuanzhike.top/gtarrzcqhy.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zhiwuduotai.top/gtuykwffqf.html

[R14] C 风格 for
来源：http://hz.cdnleiting.top/gthgclqral.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.dianchejie.cn/gtvcwanpqi.html

[R15] while 逐行读文件
来源：http://hz.fzhhl.top/gtvukwcxqw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aizwys.cn/gtsslalnfy.html

[R16] until 等待条件
来源：http://hz.shzxlz.cn/gtsndvcazn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gzhubu.top/gtnaoihvad.html

[R17] 数组定义与取值
来源：http://hz.aizwys.cn/gtxphjreds.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.mhx1999.top/gtfhbldvbu.html

[R18] 遍历数组
来源：http://hz.yueranfly.top/gtijkrqzcs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yvedp.cn/gtencvrnjn.html

[R19] 数组长度
来源：http://hz.jyoumei.cn/gtfmpwnebh.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gthdgbanqh.html

[R20] 关联数组（字典）
来源：http://hz.xinyue.icu/gtlyoyxqil.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.zhiwuduotai.top/gtakqdypyq.html

[R21] 字符串长度
来源：http://hz.jianghu66.top/gttnyddcyl.html

echo "${#s}"
来源：http://hz.smart0.xyz/gtlyelyirn.html

[R22] 截取子串
来源：http://hz.sweek.top/gtrazclhtp.html

echo "${s:0:5}"
来源：http://hz.xziqi.cn/gtkoxuffhc.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtryiokcco.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.chenjidiqi.icu/gtxnixsens.html

[R24] 大小写转换
来源：http://hz.zhengqikj.top/gtaoczoipr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.ehwqpu.com/gtdqvdwmrb.html

[R25] 去后缀 / 去前缀
来源：http://hz.cheryme.top/gtvrlfjrtb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dashuyun.cn/gtyfvpzyca.html

[R26] 命令替换
来源：http://hz.guowangkeji.top/gthbhprclh.html

now=$(date +%F); echo "$now"
来源：http://hz.52xcode.cn/gtxxvyqhcm.html

[R27] 算术展开
来源：http://hz.yangfankeji.com/gtbscbnivw.html

echo $((1 + 2 * 3))
来源：http://hz.ydzc1.top/gtrxpladwv.html

[R28] 浮点运算
来源：http://hz.ydzc1.top/gtsufdfawf.html

echo "scale=2; 10/3" | bc
来源：http://hz.pengpengdd.cyou/gtmegypppl.html

[R29] 定义函数
来源：http://hz.jiagoushi.top/gthtrtxxqo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.dianchejie.cn/gtfhznogev.html

[R30] 函数返回状态码
来源：http://hz.cqqwz.cn/gtowmnjaaf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.hammf.cn/gtulrasoyq.html

[R31] 局部变量
来源：http://hz.yueranfly.top/gtswqvnkyv.html

f() { local x=1; echo "$x"; }
来源：http://hz.shangyingyoupin.top/gtxjhhpide.html

[R32] 参数个数校验
来源：http://hz.quarkkingdee.top/gtrrglyxfo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ppjwa.cn/gtbwdxhwcm.html

[R33] 捕获错误并提示行号
来源：http://hz.hnqzz.top/gtlbjiuedn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shzxlz.cn/gtmszmuoyh.html

[R34] 退出时清理
来源：http://hz.316326.xyz/gtozmooiug.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sweek.top/gtkddbauao.html

[R35] 后台执行并等待
来源：http://hz.tianlin.xyz/gtsnmszvrr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.c1oappe.top/gtifqgfbjf.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtrivsprte.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jqgfzy.top/gtfmrkqrpd.html

[R37] 把输出赋给变量
来源：http://hz.nanxinkj.top/gthkkjydgx.html

files=$(ls -1)
来源：http://hz.cucudq.cn/gtglqzlbnb.html

[R38] 管道串联
来源：http://hz.bjfxy.top/gtmdgwewnl.html

cat a.txt | grep -i error | wc -l
来源：http://hz.jinghuilouyu.cn/gtffrxqqqd.html

[R39] 重定向标准输出与错误
来源：http://hz.chenlongwang.top/gtflnkhvdr.html

cmd > out.log 2>&1
来源：http://hz.smart0.xyz/gtbhvvdbna.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtfonhtcdf.html

echo "log" >> out.log
来源：http://hz.andypj.xyz/gtxgkcxyof.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtcaxfgqdb.html

cmd >/dev/null 2>&1
来源：http://hz.sxryk.cn/gtofsqzotu.html

[R42] 输入重定向
来源：http://hz.zhongyouzk.top/gtdwyuazob.html

wc -l < a.txt
来源：http://hz.havefunace.top/gthfibiqxz.html

[R43] 按名字查找文件
来源：http://hz.nanxinkj.top/gtwrcamsrm.html

find . -name "*.log" -type f
来源：http://hz.cucudq.cn/gtmbobboao.html

[R44] 按修改时间查找
来源：http://hz.xuetiantiany.cn/gtieiwiqlv.html

find . -mtime -7 -type f
来源：http://hz.52xcode.cn/gtltmjkbdh.html

[R45] 批量删除
来源：http://hz.yongpay.top/gtlgaiocoi.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258888.top/gtzrxioyhk.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtbfxunxwi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.meibo888.top/gtbfjdwydl.html

[R47] sed 单行替换
来源：http://hz.aibaodan.cn/gtkcavqbsy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ydjk.org.cn/gttutbkjil.html

[R48] awk 取指定列
来源：http://hz.xuetiantiany.cn/gtjtzkpicj.html

awk '{print $1, $3}' a.txt
来源：http://hz.cucudq.cn/gtajhlzilg.html

[R49] awk 带条件
来源：http://hz.hnxiangtu.top/gtminquiod.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.aizwys.cn/gtwxxsogmh.html

[R50] awk 求和
来源：http://hz.daxiang520.top/gtixeshuhw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.bjfxy.top/gtzplpcshw.html

[R51] 排序去重取前几
来源：http://hz.bjfxy.top/gtoeflnjnf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtrpvdayoc.html

[R52] 统计行数
来源：http://hz.kuanghao11.cn/gtraxidgyw.html

wc -l a.txt
来源：http://hz.yuxming.cn/gttfabanmj.html

[R53] 查看文件头与实时尾
来源：http://hz.kuanghao11.cn/gtmjsckvbk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hysaishi.cn/gtbtcsdzyl.html

[R54] 比较两个文件
来源：http://hz.cdnleiting.top/gtwsfctbdy.html

diff a.txt b.txt
来源：http://hz.ybcxt.top/gteamefolz.html

[R55] 压缩与解压
来源：http://hz.cdnleiting.top/gtnwsckfsb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.nanxuanxn.top/gtyiomuqyr.html

[R56] 远程拷贝
来源：http://hz.bjfxy.top/gtyywgxmje.html

scp file user@host:/path/
来源：http://hz.svipenyu.cn/gtyetvqdiy.html

[R57] 远程执行命令
来源：http://hz.ehwqpu.com/gtiyvrjbrp.html

ssh user@host 'uptime'
来源：http://hz.cqqwz.cn/gtbvsubeym.html

[R58] 下载文件
来源：http://hz.zycfv.cn/gtsweecmdq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuetiantiany.cn/gtgqvifmyo.html

[R59] 发 POST JSON
来源：http://hz.tian-w.cn/gtohtktpiy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtdnylyccr.html

[R60] 只看 HTTP 状态码
来源：http://hz.jqgfzy.top/gtghvmjqnz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.andypj.xyz/gtstrcsywk.html

[R61] 磁盘占用
来源：http://hz.yuxming.cn/gtizqxptru.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gtrwqxjloa.html

[R62] 找最占空间的文件
来源：http://hz.xuanzx.com/gtbmxjzqpe.html

du -ah . | sort -rh | head -10
来源：http://hz.yangfankeji.com/gtvwmixgyl.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gtiqzekfse.html

free -h;  ps aux | grep nginx
来源：http://hz.dianchejie.cn/gtfkhyengr.html

[R64] 结束进程
来源：http://hz.fzhhl.top/gtabnpjktz.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shanyushiyangkeji.top/gtjzlqtqdp.html

[R65] 查看端口占用
来源：http://hz.yongpay.top/gtkehhmmgh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.sufxvd.cn/gtmtjzblgr.html

[R66] 定时任务
来源：http://hz.aibaodan.cn/gthpxnhbkn.html

crontab -e;  crontab -l
来源：http://hz.yj20258888.top/gtoytlhuji.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtwwfufven.html

openssl rand -hex 16
来源：http://hz.meibo888.top/gtdycfeilp.html

[R68] 计算文件校验值
来源：http://hz.cqqwz.cn/gtkrqszoov.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.redwolf501.top/gtbcrwchqs.html

[R69] 生成随机密码
来源：http://hz.havefunace.top/gtiqkavxvh.html

head -c 16 /dev/urandom | base64
来源：http://hz.shangyingyoupin.top/gtqqvlzolg.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtpvjxjegv.html

date +%s;  date -d @1700000000
来源：http://hz.jinyuanbaomall.cn/gtvekkkakn.html

[R71] 日期格式化
来源：http://hz.yueranfly.top/gtpipmlauu.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.iojbl.cn/gtptlxkiqn.html

[R72] 等待端口就绪
来源：http://hz.gogol.net.cn/gtxfftsebl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtdetlcbhw.html

[R73] 分割大日志
来源：http://hz.jqgufenzy.top/gtfxtmvguj.html

split -l 1000 big.log part_
来源：http://hz.gogol.net.cn/gtihabtsci.html

[R74] 批量重命名
来源：http://hz.hongshengwenyu.top/gtuugmfftu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.kuanghao11.cn/gtbnoyepjc.html

[R75] 导出环境变量
来源：http://hz.kuanghao11.cn/gtwzdwdqas.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhixingplan.top/gtsranzqpw.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtjenksnld.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.shangyingyoupin.top/gtjzrfueyz.html

[R77] 读取用户输入
来源：http://hz.meibo888.top/gtznjyekvc.html

read -rp "请输入: " ans
来源：http://hz.zhijiandao.cn/gtgbahnkxn.html

[R78] 交互式菜单
来源：http://hz.chenlongwang.top/gtesucovro.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.guowangkeji.top/gtwgaopzrd.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangtech.top/gtclbwolxx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.shanyushiyangkeji.top/gtptsnvyde.html

[R80] 查看脚本执行耗时
来源：http://hz.sysykeji.top/gtwzjlhrea.html

time ./run.sh
来源：http://hz.ydzc1.top/gtmohhcsvu.html

================================================================================
来源：http://hz.chenjidiqi.icu/gtvqczjelq.html

S. C / C++ 专题
来源：http://hz.52xcode.cn/gturaxsjwu.html

================================================================================
来源：http://hz.mhx1999.top/gtyagguvxm.html

[S01] C：Hello World
来源：http://hz.wangshuangyany.cn/gtqsipnyrj.html

#include <stdio.h>
来源：http://hz.xingfuxueyuan.xyz/gthtdtaylu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hnqzz.top/gtsyymxxny.html

[S02] C：变量与格式化输出
来源：http://hz.shangyingyoupin.top/gtqysafjso.html

int a = 10; printf("%d\n", a);
来源：http://hz.jiagoushi.top/gtyzxitsoa.html

[S03] C：读入整数
来源：http://hz.jlsjyb.cn/gtdzdljsnr.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gtmzcitpan.html

[S04] C：字符串复制
来源：http://hz.guannengcc.top/gtbndbyqvb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.iojbl.cn/gtsejpoxso.html

[S05] C：字符串长度
来源：http://hz.xziqi.cn/gtkoemtmoi.html

strlen(s)
来源：http://hz.bjfxy.top/gtyhdjvuon.html

[S06] C：字符串比较
来源：http://hz.cqqwz.cn/gtnvboiiop.html

strcmp(a, b) == 0
来源：http://hz.jinqigfzy.top/gtlfuyfpab.html

[S07] C：数组遍历求和
来源：http://hz.xuetiantiany.cn/gtlzmojnel.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aizwys.cn/gtxbstoqwv.html

[S08] C：动态内存分配与释放
来源：http://hz.pengpengdd.cyou/gtinwwfftg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhoulong.xyz/gtrupdgyzu.html

[S09] C：结构体定义与初始化
来源：http://hz.ywan-chungtsiang.top/gtexwsmtcq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.yueranfly.top/gtdkyxymlf.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtvvomohsn.html

int *p = &a;  *p = 5;
来源：http://hz.daria6918.cn/gtzdahunlm.html

[S11] C：逐行读文件
来源：http://hz.jinqigufen.top/gtpbdoomwx.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cdnleiting.top/gtabfkcrjt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258.top/gtlnroivgg.html

fclose(f);
来源：http://hz.nanxinkj.top/gttohiajxt.html

[S12] C：写文件
来源：http://hz.pycfn.com/gtkqlziwvw.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jiagoushi.top/gtdnqenzhj.html

[S13] C：宏定义
来源：http://hz.zdqjudy.top/gtkyrnlwsb.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.chenzaomai.com/gtrmeogyrz.html

[S14] C：枚举
来源：http://hz.andypj.xyz/gttlakwnga.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.316326.xyz/gtkykagxyk.html

[S15] C：类型转换
来源：http://hz.wangdashe.top/gtcaygxlaj.html

(double) a / b
来源：http://hz.yuxming.cn/gtngwgwvjj.html

[S16] C：位操作置位
来源：http://hz.zhaomingkeji.xyz/gtdwrkceef.html

x |= (1 << 3);
来源：http://hz.cdnleiting.top/gtmekbzchy.html

[S17] C：安全拼接字符串
来源：http://hz.zhixingplan.top/gtehpzwqxi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.xylfe.cn/gtkyrwjucb.html

[S18] C：命令行参数
来源：http://hz.yangfankeji.com/gttmwywpvh.html

int main(int argc, char **argv)
来源：http://hz.gzhubu.top/gtfaocgvvz.html

[S19] C：快速排序
来源：http://hz.yonumen.top/gtoibemean.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yvedp.cn/gteehfslcg.html

[S20] C：二分查找
来源：http://hz.bjfxy.top/gttcgphult.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtheeummvt.html

[S21] C：字符类别判断
来源：http://hz.zdqjudy.top/gtgmdevamz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.kuanghao11.cn/gtvxyssvsw.html

[S22] C：字符串转数字
来源：http://hz.zycfv.cn/gtxakwqgvz.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.c1oappe.top/gtlzffnwxq.html

[S23] C：随机数
来源：http://hz.ywan-chungtsiang.top/gtihfckxgm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.jqgfzy.top/gtwlowrsvx.html

[S24] C：获取本地时间
来源：http://hz.yanxiufei.cn/gthriuynql.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangshuangyany.cn/gtieqryofq.html

[S25] C：内存拷贝
来源：http://hz.yanxiufei.cn/gtrmkrcryu.html

memcpy(dst, src, n);
来源：http://hz.chenzaomai.com/gtjrziexrg.html

[S26] C：内存清零
来源：http://hz.jinqigufen.top/gtmuomhigq.html

memset(a, 0, sizeof a);
来源：http://hz.iojbl.cn/gtetfnanzp.html

[S27] C：定义常量
来源：http://hz.jlsjyb.cn/gtyhviuzty.html

const double PI = 3.14159;
来源：http://hz.hongshengwenyu.top/gtjpnpimkq.html

[S28] C：静态变量
来源：http://hz.yongpay.top/gtbbtfywnq.html

static int counter = 0;
来源：http://hz.hnxiangtu.top/gtbqimmqtz.html

[S29] C：变参函数
来源：http://hz.zhiwuduotai.top/gteecmmtbr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xylfe.cn/gtccftwfsy.html

[S30] C：头文件保护
来源：http://hz.cheryme.top/gthocpqcfh.html

#ifndef X_H
来源：http://hz.cdnleiting.top/gtjvszihwn.html

#define X_H
来源：http://hz.pycfn.com/gtiybyclgl.html

#endif
来源：http://hz.zhiwuduotai.top/gtsjcsjyjr.html

[S31] C++：Hello World
来源：http://hz.havefunace.top/gtzlwlqgwz.html

#include <iostream>
来源：http://hz.0kj1m.cn/gtpobcopzz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.ywan-chungtsiang.top/gtchawsbnv.html

[S32] C++：字符串
来源：http://hz.yj20258.top/gtyuxgwovv.html

std::string s = "hi";  s += "!";
来源：http://hz.yvedp.cn/gtjvknzewj.html

[S33] C++：vector 增删
来源：http://hz.zhaomingkeji.xyz/gteegwjacg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.iojbl.cn/gteufrkqlc.html

[S34] C++：遍历 vector
来源：http://hz.kuanghao11.cn/gtxeriesnb.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.sufxvd.cn/gthsnjnyir.html

[S35] C++：map
来源：http://hz.xuanzx.com/gtftdngvel.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.nwbrower.top/gtkyzrldeq.html

[S36] C++：unordered_map
来源：http://hz.quarkkingdee.top/gtlljzfzdk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.wangshuangyany.cn/gtbsgeesfi.html

[S37] C++：set
来源：http://hz.yuxming.cn/gtzndbpxpj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.quarkkingdee.top/gttoivwlgj.html

[S38] C++：排序
来源：http://hz.shzxlz.cn/gtyrrqoipq.html

std::sort(v.begin(), v.end());
来源：http://hz.pycfn.com/gtujoqxusf.html

[S39] C++：自定义比较器排序
来源：http://hz.sxryk.cn/gtcbmcwpqs.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.havefunace.top/gtcbzcutin.html

[S40] C++：查找元素
来源：http://hz.iojbl.cn/gtalbjouvw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yanxiufei.cn/gtrbmliwhd.html

[S41] C++：类与构造函数
来源：http://hz.pengpengdd.cyou/gtsqixhcls.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.andypj.xyz/gtlvsnilps.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtlbjjjmxv.html

class B : public Base { public: void f() override {} };
来源：http://hz.andypj.xyz/gtxpbhbwdi.html

[S43] C++：智能指针
来源：http://hz.nanxuanxn.top/gtljvomcty.html

auto p = std::make_unique<int>(5);
来源：http://hz.gzhubu.top/gtfepgjljf.html

[S44] C++：引用传参
来源：http://hz.shanyushiyangkeji.top/gtnyyjrcdl.html

void inc(int &x) { ++x; }
来源：http://hz.jiagoushi.top/gtkcjyaykg.html

[S45] C++：lambda
来源：http://hz.ehwqpu.com/gtnjnnqjsv.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.aibaodan.cn/gtzrsmrvle.html

[S46] C++：函数模板
来源：http://hz.jinghuilouyu.cn/gtgwsjxthw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jqgfzy.top/gttohkwkyv.html

[S47] C++：结构化绑定遍历
来源：http://hz.0kj1m.cn/gtreeoplqc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.birdmap.top/gtmdltwitj.html

[S48] C++：逐行读文件
来源：http://hz.cheryme.top/gtlopbiivc.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.cqqwz.cn/gtjgcvsqtt.html

while (std::getline(in, line)) { }
来源：http://hz.yj20258.top/gtjqrehgwg.html

[S49] C++：写文件
来源：http://hz.jinghuilouyu.cn/gtvlzaizjr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hnqzz.top/gthmnrvrgx.html

[S50] C++：格式化数字
来源：http://hz.shanyushiyangtech.top/gtvpoarbnd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.nanxinkj.top/gtjwjseprn.html

[S51] C++：显式类型转换
来源：http://hz.sweek.top/gteqpywfks.html

static_cast<double>(a) / b
来源：http://hz.fengsongda.top/gtgzqrlfyj.html

[S52] C++：const 与 noexcept
来源：http://hz.yj20258.top/gtchevatfd.html

int size() const noexcept { return n_; }
来源：http://hz.xingfuxueyuan.xyz/gtgstbxsjr.html

[S53] C++：移动语义
来源：http://hz.yongpay.top/gtfzgwxdif.html

std::vector<int> w = std::move(v);
来源：http://hz.mhx1999.top/gtvtosdznd.html

[S54] C++：异常处理
来源：http://hz.guannengcc.top/gtvxsakiwu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.jinqigufen.top/gtyaqexwxw.html

[S55] C++：结构化绑定
来源：http://hz.jinghuilouyu.cn/gtdxoduydm.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jqgfzy.top/gtmaoarwwc.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtlrcxqgni.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.9152youxi.cn/gthgnzwdhj.html

[S57] C++：编译期常量
来源：http://hz.andypj.xyz/gtieuenvgp.html

constexpr int N = 10;
来源：http://hz.zhengqikj.top/gtqddftuyo.html

[S58] C++：命名空间
来源：http://hz.shangyingyoupin.top/gtnwnxqpcn.html

namespace ns { int f() { return 1; } }
来源：http://hz.fzhhl.top/gtldvfnqnu.html

[S59] C++：静态断言
来源：http://hz.haohaochexian.top/gtezyrxtol.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.xuanzx.com/gtryceytnw.html

[S60] C++：遍历并删除元素
来源：http://hz.hfpthk.cn/gtkvlequxh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.cashguo.top/gtcdlvwxgh.html

================================================================================
来源：http://hz.jqgfzy.top/gtitkosszk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.9152youxi.cn/gtrsyrfgwl.html

================================================================================
来源：http://hz.yangfankeji.com/gtokgoettw.html

[T01] Kotlin：Hello World
来源：http://hz.guowangkeji.top/gthmuijmyr.html

println("Hello")
来源：http://hz.cashguo.top/gtbpvsdbtz.html

[T02] Kotlin：变量
来源：http://hz.nwbrower.top/gtmdufokkl.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.shanyushiyangtech.top/gtaggjqqra.html

[T03] Kotlin：字符串模板
来源：http://hz.jlsjyb.cn/gthbdiwtfx.html

"值: $b"
来源：http://hz.gotoacloud.top/gttwtzcfkh.html

[T04] Kotlin：空安全
来源：http://hz.9152youxi.cn/gtsvkrjdmr.html

val n: String? = null;  n?.length
来源：http://hz.redwolf501.top/gtwsdrmqim.html

[T05] Kotlin：when 表达式
来源：http://hz.yj202588.top/gttuwjsfdb.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.vqdsnc.cn/gtntzxdzvj.html

[T06] Kotlin：集合映射
来源：http://hz.dianchejie.cn/gtdaeplfic.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.hfpthk.cn/gtsdajwrxw.html

[T07] Kotlin：集合过滤
来源：http://hz.yonumen.top/gtpbjmensj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yj202588.top/gtrmuqrtfg.html

[T08] Kotlin：数据类
来源：http://hz.quarkkingdee.top/gtiiadyrqx.html

data class User(val name: String, val age: Int)
来源：http://hz.jqgufenzy.top/gtsldfzyyz.html


<!-- 参考信息 -->