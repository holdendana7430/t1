代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtplvqlwei.html

[R10] 正则匹配
来源：http://hz.xuetiantiany.cn/gthmqeehyz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.chenzaomai.com/gtxbaxzuas.html

[R11] case 多分支
来源：http://hz.jianghu66.top/gtqkxwpruu.html

case "$1" in
来源：http://hz.guowangkeji.top/gtuvjnmkmq.html

start) echo "启动" ;;
来源：http://hz.tian-w.cn/gtycpxtlqm.html

stop)  echo "停止" ;;
来源：http://hz.52xcode.cn/gtwhbaihem.html

*)     echo "未知命令" ;;
来源：http://hz.smart0.xyz/gtzxpmufrp.html

esac
来源：http://hz.guowangkeji.top/gtpmxcgmum.html

[R12] for 遍历文件
来源：http://hz.zhongyouzk.top/gtqwogfxar.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yvedp.cn/gtibkowgnf.html

[R13] for 计数循环
来源：http://hz.fzhhl.top/gtrdvyypbk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.ppjwa.cn/gtkaeectlb.html

[R14] C 风格 for
来源：http://hz.guowangkeji.top/gtosfdvics.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.feifeiyinyue.top/gtrmzfkvoe.html

[R15] while 逐行读文件
来源：http://hz.tanke756.top/gtmqjxffdl.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yanxiufei.cn/gtxgpdvmxh.html

[R16] until 等待条件
来源：http://hz.shzxlz.cn/gtzrkkxvsh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ivvv.top/gtewnqpfax.html

[R17] 数组定义与取值
来源：http://hz.aibaodan.cn/gtbrmogavq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.ydjk.org.cn/gtoheimfuy.html

[R18] 遍历数组
来源：http://hz.iojbl.cn/gtbpixurqi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.daria6918.cn/gtterqdayy.html

[R19] 数组长度
来源：http://hz.316326.xyz/gtndybkbtc.html

echo "${#arr[@]}"
来源：http://hz.dianchejie.cn/gtsnrvkmhv.html

[R20] 关联数组（字典）
来源：http://hz.ehwqpu.com/gtekgugidt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yongpay.top/gtqpbucple.html

[R21] 字符串长度
来源：http://hz.9152youxi.cn/gtvmgyuzeg.html

echo "${#s}"
来源：http://hz.dianchejie.cn/gtrmokxoed.html

[R22] 截取子串
来源：http://hz.dianchejie.cn/gttkebnmdx.html

echo "${s:0:5}"
来源：http://hz.jyoumei.cn/gthelslxrr.html

[R23] 字符串替换
来源：http://hz.tianlin.xyz/gtwdvmgtpn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.shangyingyoupin.top/gtaorakeor.html

[R24] 大小写转换
来源：http://hz.hfpthk.cn/gtkemhmglp.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.jqgfzy.top/gtauiojwqg.html

[R25] 去后缀 / 去前缀
来源：http://hz.yueranfly.top/gtrrqxhtee.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtozfvolqa.html

[R26] 命令替换
来源：http://hz.jiagoushi.top/gtouoadjyk.html

now=$(date +%F); echo "$now"
来源：http://hz.ywan-chungtsiang.top/gtlolnloeb.html

[R27] 算术展开
来源：http://hz.bjfxy.top/gtqlxnwogv.html

echo $((1 + 2 * 3))
来源：http://hz.sxryk.cn/gtasokuzfq.html

[R28] 浮点运算
来源：http://hz.52xcode.cn/gtrrdzvzux.html

echo "scale=2; 10/3" | bc
来源：http://hz.52xcode.cn/gtzasukpri.html

[R29] 定义函数
来源：http://hz.zhiwuduotai.top/gtrmcqxyqo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.svipenyu.cn/gtvpiysucq.html

[R30] 函数返回状态码
来源：http://hz.ppjwa.cn/gtshydvouk.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yongpay.top/gtgoorhzzd.html

[R31] 局部变量
来源：http://hz.shanyushiyangkeji.top/gtcoxdbtli.html

f() { local x=1; echo "$x"; }
来源：http://hz.guowangkeji.top/gtxdpwyysh.html

[R32] 参数个数校验
来源：http://hz.ydjk.org.cn/gthfpjwopa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.redwolf501.top/gtyurpbrrl.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtnkvwjhfd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ybcxt.top/gtvacjvrns.html

[R34] 退出时清理
来源：http://hz.xziqi.cn/gtrkmkprhu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.hnxiangtu.top/gtnbzutscz.html

[R35] 后台执行并等待
来源：http://hz.zhaomingkeji.xyz/gtqznwihqx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.yj202588.top/gtrwmfpiwd.html

[R36] 并发执行多个任务
来源：http://hz.pycfn.com/gtmsfqapyv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.mhx1999.top/gtspwacckb.html

[R37] 把输出赋给变量
来源：http://hz.yj20258.top/gtyloataxj.html

files=$(ls -1)
来源：http://hz.jinghuilouyu.cn/gtnltgryju.html

[R38] 管道串联
来源：http://hz.tianlin.xyz/gtppsalqku.html

cat a.txt | grep -i error | wc -l
来源：http://hz.bjfxy.top/gtczrdhyiw.html

[R39] 重定向标准输出与错误
来源：http://hz.daria6918.cn/gtssupitvg.html

cmd > out.log 2>&1
来源：http://hz.mhx1999.top/gtzkvhhuuz.html

[R40] 追加写日志
来源：http://hz.gogol.net.cn/gtwwmwqvxa.html

echo "log" >> out.log
来源：http://hz.dianchejie.cn/gtzwnxwbwi.html

[R41] 丢弃输出
来源：http://hz.c1oappe.top/gtrsktosnt.html

cmd >/dev/null 2>&1
来源：http://hz.zhengqikj.top/gtzmcsbdrj.html

[R42] 输入重定向
来源：http://hz.haohaochexian.top/gtjuwftlrs.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtsghpogic.html

[R43] 按名字查找文件
来源：http://hz.gogol.net.cn/gtsokgkkqv.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtxhdyoset.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gthvmzeqdp.html

find . -mtime -7 -type f
来源：http://hz.nanxuanxn.top/gtvutstsxg.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtpcozjfaw.html

find . -name "*.tmp" -delete
来源：http://hz.haohaochexian.top/gtmeheltzi.html

[R46] 递归替换文件内容
来源：http://hz.svipenyu.cn/gthaektolw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.hfpthk.cn/gtlrotlrgl.html

[R47] sed 单行替换
来源：http://hz.kuanghao11.cn/gtvmrfnwbm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.daxiang520.top/gtllxzdqnx.html

[R48] awk 取指定列
来源：http://hz.xinyue.icu/gtitjfdhnh.html

awk '{print $1, $3}' a.txt
来源：http://hz.jinqigfzy.top/gtmfruccgs.html

[R49] awk 带条件
来源：http://hz.haohaochexian.top/gtffsvscwm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhengqikj.top/gtumhruzrl.html

[R50] awk 求和
来源：http://hz.jinyuanbaomall.cn/gtavavaaks.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtgagnbblq.html

[R51] 排序去重取前几
来源：http://hz.yj20258.top/gtkjwkerwf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtybeopphv.html

[R52] 统计行数
来源：http://hz.iojbl.cn/gtcvppvdhj.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gtscgwgpow.html

[R53] 查看文件头与实时尾
来源：http://hz.ydzc1.top/gteeypifwl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.daxiang520.top/gtaiquuqol.html

[R54] 比较两个文件
来源：http://hz.ydzc1.top/gtasqnkryk.html

diff a.txt b.txt
来源：http://hz.shanyushiyangkeji.top/gtwmaelzku.html

[R55] 压缩与解压
来源：http://hz.shuidangran.top/gtkogfkcio.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.daxiang520.top/gteivihprl.html

[R56] 远程拷贝
来源：http://hz.cdnleiting.top/gtvdtgdzpz.html

scp file user@host:/path/
来源：http://hz.jlsjyb.cn/gtqipewxwb.html

[R57] 远程执行命令
来源：http://hz.aibaodan.cn/gthysusbpw.html

ssh user@host 'uptime'
来源：http://hz.mhx1999.top/gtojxfjzcl.html

[R58] 下载文件
来源：http://hz.zhaomingkeji.xyz/gtxqwmyamf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.ybcxt.top/gteiqzjatf.html

[R59] 发 POST JSON
来源：http://hz.chenlongwang.top/gththttilk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinqigfzy.top/gtdkemjviq.html

[R60] 只看 HTTP 状态码
来源：http://hz.9152youxi.cn/gtacmxaown.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.birdmap.top/gtdfubkffv.html

[R61] 磁盘占用
来源：http://hz.316326.xyz/gtpvkapiih.html

df -h;  du -sh *
来源：http://hz.9152youxi.cn/gtkizwfowo.html

[R62] 找最占空间的文件
来源：http://hz.feifeiyinyue.top/gtidogphwy.html

du -ah . | sort -rh | head -10
来源：http://hz.kuanghao11.cn/gtwzgzdbbl.html

[R63] 内存与进程
来源：http://hz.daxiang520.top/gtondeoqud.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gtzpkyauki.html

[R64] 结束进程
来源：http://hz.jinyuanbaomall.cn/gtpmhpiosq.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fengsongda.top/gtgqkrxxrb.html

[R65] 查看端口占用
来源：http://hz.jinghuilouyu.cn/gtuxmvtqvy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gzhubu.top/gtkmegiesf.html

[R66] 定时任务
来源：http://hz.ydjk.org.cn/gtzepegmsx.html

crontab -e;  crontab -l
来源：http://hz.quarkkingdee.top/gtrsvkggmf.html

[R67] 生成随机十六进制串
来源：http://hz.nanxinkj.top/gtpzyxfbph.html

openssl rand -hex 16
来源：http://hz.feifeiyinyue.top/gtolickkjx.html

[R68] 计算文件校验值
来源：http://hz.birdmap.top/gtkilfwdxz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hongshengwenyu.top/gtrdmsvqpf.html

[R69] 生成随机密码
来源：http://hz.9152youxi.cn/gtefceathw.html

head -c 16 /dev/urandom | base64
来源：http://hz.quarkkingdee.top/gtnqnutwda.html

[R70] 时间戳与互转
来源：http://hz.cheryme.top/gtlpyhslsg.html

date +%s;  date -d @1700000000
来源：http://hz.chenlongwang.top/gtrhzmzpci.html

[R71] 日期格式化
来源：http://hz.gogol.net.cn/gtfcixwvcz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jqgufenzy.top/gtdbxwhnvh.html

[R72] 等待端口就绪
来源：http://hz.zhaomingkeji.xyz/gtqbskcdsl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.yuanzhike.top/gtuxtzkkfy.html

[R73] 分割大日志
来源：http://hz.gzhubu.top/gtqvdloivt.html

split -l 1000 big.log part_
来源：http://hz.316326.xyz/gtwgsahubb.html

[R74] 批量重命名
来源：http://hz.ybcxt.top/gtuxsjitpr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hnqzz.top/gtziebcede.html

[R75] 导出环境变量
来源：http://hz.ybcxt.top/gtsblwuwlj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhaomingkeji.xyz/gtsbznnkgv.html

[R76] 使用临时文件
来源：http://hz.c1oappe.top/gtdsdvpste.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.hongshengwenyu.top/gtpmwsbyze.html

[R77] 读取用户输入
来源：http://hz.shangyingyoupin.top/gtkwkcaibs.html

read -rp "请输入: " ans
来源：http://hz.ivvv.top/gtucoqfmmv.html

[R78] 交互式菜单
来源：http://hz.shangyingyoupin.top/gtexvamqnt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nanxinkj.top/gtdjqarffz.html

[R79] 解析命令行选项
来源：http://hz.gaohongyu789.top/gteuvxsftl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.52xcode.cn/gtxnpbxfcg.html

[R80] 查看脚本执行耗时
来源：http://hz.iojbl.cn/gtxxuhqtjy.html

time ./run.sh
来源：http://hz.hongshengwenyu.top/gtioavjndo.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtapoiaubf.html

S. C / C++ 专题
来源：http://hz.xinyue.icu/gtgfjsawnb.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtwpqeztss.html

[S01] C：Hello World
来源：http://hz.gzhubu.top/gtmojeyedq.html

#include <stdio.h>
来源：http://hz.hfpthk.cn/gtyzbdncnr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtprksnekz.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtitqkxaqb.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gthpkgtapx.html

[S03] C：读入整数
来源：http://hz.gogol.net.cn/gtuubqwxwg.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtjdevudxk.html

[S04] C：字符串复制
来源：http://hz.zhongyouzk.top/gtklqdjtsb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.gaohongyu789.top/gttdkcgkwm.html

[S05] C：字符串长度
来源：http://hz.hfpthk.cn/gtsscuptro.html

strlen(s)
来源：http://hz.snrcjt.cn/gtdhlnzrni.html

[S06] C：字符串比较
来源：http://hz.tianlin.xyz/gtbclcjvpx.html

strcmp(a, b) == 0
来源：http://hz.nanxinkj.top/gtidrbocyr.html

[S07] C：数组遍历求和
来源：http://hz.zhengqikj.top/gtatzvvkaz.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.c1oappe.top/gtgdicfboj.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtahxlvjrn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.dashuyun.cn/gtkohvocnu.html

[S09] C：结构体定义与初始化
来源：http://hz.meibo888.top/gtjqigjvqr.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.zhongyouzk.top/gtbxidaine.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtgkbfegwl.html

int *p = &a;  *p = 5;
来源：http://hz.ydzc1.top/gtffyzrrir.html

[S11] C：逐行读文件
来源：http://hz.zycfv.cn/gtysjwtxaf.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.hysaishi.cn/gtmdznrquv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.ydzc1.top/gtdacvbhao.html

fclose(f);
来源：http://hz.meibo888.top/gtgixwvwpm.html

[S12] C：写文件
来源：http://hz.shanyushiyangkeji.top/gtrowbeuxf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.smart0.xyz/gtmegjnbop.html

[S13] C：宏定义
来源：http://hz.hongshengwenyu.top/gtjpkiarmm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shangyingyoupin.top/gtgwvpzosm.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtiryavajk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zhoulong.xyz/gtgvnrukrn.html

[S15] C：类型转换
来源：http://hz.52xcode.cn/gthzjgaqfd.html

(double) a / b
来源：http://hz.jlsjyb.cn/gtbnunqjjh.html

[S16] C：位操作置位
来源：http://hz.sufxvd.cn/gtuljxqqpp.html

x |= (1 << 3);
来源：http://hz.quarkkingdee.top/gtalkozlnc.html

[S17] C：安全拼接字符串
来源：http://hz.vqdsnc.cn/gtajuoggji.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.nwbrower.top/gtbewhtntw.html

[S18] C：命令行参数
来源：http://hz.zhaomingkeji.xyz/gtgvguzelr.html

int main(int argc, char **argv)
来源：http://hz.hammf.cn/gtsvivqozj.html

[S19] C：快速排序
来源：http://hz.yuxming.cn/gtmqydfqwv.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.cucudq.cn/gtdgyjbixc.html

[S20] C：二分查找
来源：http://hz.chenlongwang.top/gtltwyftnf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.yuxming.cn/gtvcntytpm.html

[S21] C：字符类别判断
来源：http://hz.yangfankeji.com/gtrykagkds.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.pycfn.com/gtunxkudsx.html

[S22] C：字符串转数字
来源：http://hz.hfpthk.cn/gtywcpzmth.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtlnigsgoz.html

[S23] C：随机数
来源：http://hz.yuanzhike.top/gtfuxbmlxa.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hywenlv.cn/gtsbdpzpxx.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangkeji.top/gtdtizizia.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.hammf.cn/gtujizktdj.html

[S25] C：内存拷贝
来源：http://hz.wangdashe.top/gtmddwoqfy.html

memcpy(dst, src, n);
来源：http://hz.hnqzz.top/gtylthxpyc.html

[S26] C：内存清零
来源：http://hz.tian-w.cn/gtaxylirtr.html

memset(a, 0, sizeof a);
来源：http://hz.xinyue.icu/gtvtyjystc.html

[S27] C：定义常量
来源：http://hz.gzhubu.top/gtrmxtismo.html

const double PI = 3.14159;
来源：http://hz.52xcode.cn/gtoagjgqca.html

[S28] C：静态变量
来源：http://hz.yueranfly.top/gtoujovvvu.html

static int counter = 0;
来源：http://hz.guowangkeji.top/gtsxnnxzhw.html

[S29] C：变参函数
来源：http://hz.jianghu66.top/gtbyatoips.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.pengpengdd.cyou/gtouvssjpn.html

[S30] C：头文件保护
来源：http://hz.zhengqikj.top/gtjlityobx.html

#ifndef X_H
来源：http://hz.daxiang520.top/gtbhcegfzs.html

#define X_H
来源：http://hz.andypj.xyz/gtjdqzbvsy.html

#endif
来源：http://hz.zhoulong.xyz/gtudhdzluy.html

[S31] C++：Hello World
来源：http://hz.mhx1999.top/gtvlrwcjxb.html

#include <iostream>
来源：http://hz.guowangkeji.top/gtqeehmzlm.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.quarkkingdee.top/gtqsszpbog.html

[S32] C++：字符串
来源：http://hz.sufxvd.cn/gtusbjlgcy.html

std::string s = "hi";  s += "!";
来源：http://hz.jinqigufen.top/gtqacnkvvc.html

[S33] C++：vector 增删
来源：http://hz.sufxvd.cn/gtzgjhwlvy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.gzhubu.top/gtjonwoevn.html

[S34] C++：遍历 vector
来源：http://hz.fengsongda.top/gtjyokhkhh.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.zhengqikj.top/gtyibphlal.html

[S35] C++：map
来源：http://hz.yonumen.top/gtlxfwtttp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.chenjidiqi.icu/gtsdjgsekd.html

[S36] C++：unordered_map
来源：http://hz.gotoacloud.top/gtsctaoiex.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gaohongyu789.top/gtpxlmxcfm.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtynvfeiyl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.tian-w.cn/gtidzqsrdi.html

[S38] C++：排序
来源：http://hz.shanyushiyangtech.top/gthfzqrkvx.html

std::sort(v.begin(), v.end());
来源：http://hz.jianghu66.top/gtywqgkadl.html

[S39] C++：自定义比较器排序
来源：http://hz.dianchejie.cn/gtuxeyqixj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guowangkeji.top/gtmflygvax.html

[S40] C++：查找元素
来源：http://hz.fzhhl.top/gtpvwmlyfs.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.yangfankeji.com/gtmyoatuzb.html

[S41] C++：类与构造函数
来源：http://hz.shanyushiyangkeji.top/gtzntznlso.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.pengpengdd.cyou/gtmysjcbcb.html

[S42] C++：继承与虚函数
来源：http://hz.fzhhl.top/gtaawfqwbz.html

class B : public Base { public: void f() override {} };
来源：http://hz.smart0.xyz/gtlcydwkkr.html

[S43] C++：智能指针
来源：http://hz.daria6918.cn/gtnkbciwlz.html

auto p = std::make_unique<int>(5);
来源：http://hz.yanxiufei.cn/gtuzcomngy.html

[S44] C++：引用传参
来源：http://hz.sweek.top/gtoqqwfhnw.html

void inc(int &x) { ++x; }
来源：http://hz.jqgfzy.top/gtcpyskmze.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gtokzhjebn.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zdqjudy.top/gtmoybrdwm.html

[S46] C++：函数模板
来源：http://hz.iojbl.cn/gtowyljqcy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.shanyushiyangtech.top/gtxldqlidp.html

[S47] C++：结构化绑定遍历
来源：http://hz.jinqigufen.top/gtonelpfco.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.0kj1m.cn/gtgzujiftv.html

[S48] C++：逐行读文件
来源：http://hz.zhijiandao.cn/gtvxrvwvfh.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.yj20258888.top/gtjstjsdyy.html

while (std::getline(in, line)) { }
来源：http://hz.shangyingyoupin.top/gtllfapvqw.html

[S49] C++：写文件
来源：http://hz.redwolf501.top/gtwjrqrntm.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.yj202588.top/gthsgoywwj.html

[S50] C++：格式化数字
来源：http://hz.jianghu66.top/gtyafgvcnr.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.dianchejie.cn/gtrhpqrazi.html

[S51] C++：显式类型转换
来源：http://hz.hfpthk.cn/gtpxftkhby.html

static_cast<double>(a) / b
来源：http://hz.zhoulong.xyz/gtzdhsneap.html

[S52] C++：const 与 noexcept
来源：http://hz.hfpthk.cn/gtsbmowrlx.html

int size() const noexcept { return n_; }
来源：http://hz.xuanzx.com/gtatwwsvdy.html

[S53] C++：移动语义
来源：http://hz.sysykeji.top/gtybistszg.html

std::vector<int> w = std::move(v);
来源：http://hz.zhoulong.xyz/gthilajvsy.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gtvuctfmtv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.zhoulong.xyz/gtlozaswym.html

[S55] C++：结构化绑定
来源：http://hz.daxiang520.top/gtfcdeahwl.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.zhiwuduotai.top/gtykkdpvsy.html

[S56] C++：optional
来源：http://hz.quarkkingdee.top/gtzfhgxkln.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.xinyue.icu/gtoplbsgoa.html

[S57] C++：编译期常量
来源：http://hz.shanyushiyangkeji.top/gtokrbueju.html

constexpr int N = 10;
来源：http://hz.mhx1999.top/gtpbinkgun.html

[S58] C++：命名空间
来源：http://hz.kuanghao11.cn/gthmfjmktx.html

namespace ns { int f() { return 1; } }
来源：http://hz.snrcjt.cn/gtqkawdxgy.html

[S59] C++：静态断言
来源：http://hz.svipenyu.cn/gtjdsuymrj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.dianchejie.cn/gtrnrrpbmq.html

[S60] C++：遍历并删除元素
来源：http://hz.zhoulong.xyz/gtbnosdpkl.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.ydzc1.top/gtwbutdbnb.html

================================================================================
来源：http://hz.yuxming.cn/gtahalense.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.mhx1999.top/gtzbbwlgyy.html

================================================================================
来源：http://hz.xinyue.icu/gtflbmdmqg.html

[T01] Kotlin：Hello World
来源：http://hz.316326.xyz/gtmacltppt.html

println("Hello")
来源：http://hz.chenzaomai.com/gtprmhpppy.html

[T02] Kotlin：变量
来源：http://hz.sysykeji.top/gtcicsznnq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.svipenyu.cn/gtidrdmlss.html

[T03] Kotlin：字符串模板
来源：http://hz.xuanzx.com/gthuykuode.html

"值: $b"
来源：http://hz.iojbl.cn/gtolwuefaj.html

[T04] Kotlin：空安全
来源：http://hz.shanyushiyangkeji.top/gtygubpnev.html

val n: String? = null;  n?.length
来源：http://hz.yangfankeji.com/gtatfhqllw.html

[T05] Kotlin：when 表达式
来源：http://hz.tanke756.top/gtnxphecgy.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.xziqi.cn/gtzoctqdkb.html

[T06] Kotlin：集合映射
来源：http://hz.ydzc1.top/gtnbtjxgpg.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.bjfxy.top/gthhzpsxlh.html

[T07] Kotlin：集合过滤
来源：http://hz.tanke756.top/gtghbvdopc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.yuanzhike.top/gtrfthilhl.html

[T08] Kotlin：数据类
来源：http://hz.pycfn.com/gtwgfnpysy.html

data class User(val name: String, val age: Int)
来源：http://hz.fengsongda.top/gtqzzdpjsw.html

[T09] Kotlin：扩展函数
来源：http://hz.zdqjudy.top/gtvrrnbwwb.html

fun String.exclaim() = this + "!"
来源：http://hz.aibaodan.cn/gtfegkhzcc.html

[T10] Kotlin：默认参数
来源：http://hz.vqdsnc.cn/gthroujhcq.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.wangdashe.top/gtmrkxclef.html


<!-- 参考信息 -->