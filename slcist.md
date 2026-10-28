代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jinghuilouyu.cn/gtxybqcare.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangkeji.top/gtucvlbpzj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shuidangran.top/gtgxnejnyf.html

================================================================================
来源：http://hz.yuxming.cn/gtxarsbcng.html

R. Bash 专题
来源：http://hz.cqqwz.cn/gtmzxtcvob.html

================================================================================
来源：http://hz.tian-w.cn/gttgavhamk.html

[R01] shebang 与严格模式
来源：http://hz.xylfe.cn/gtoivxovcf.html

#!/usr/bin/env bash
来源：http://hz.chenlongwang.top/gthztjexbl.html

set -euo pipefail
来源：http://hz.gzhubu.top/gtytwiucvn.html

[R02] 变量赋值与使用
来源：http://hz.cdnleiting.top/gtzufwllpo.html

name="Tom"; echo "$name"
来源：http://hz.pengpengdd.cyou/gtzwgzhrvj.html

[R03] 只读变量
来源：http://hz.xziqi.cn/gtureuyooe.html

readonly PI=3.14
来源：http://hz.ivvv.top/gtzoolezcb.html

[R04] 位置参数
来源：http://hz.ydjk.org.cn/gtalippska.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xziqi.cn/gtfbfzmsrc.html

[R05] 参数默认值
来源：http://hz.zdqjudy.top/gtzaozfcdo.html

name="${1:-default}"
来源：http://hz.zhengqikj.top/gtgvkfdjro.html

[R06] 判断命令是否存在
来源：http://hz.jqgufenzy.top/gtoqksuuzn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.smart0.xyz/gtqscmxgsj.html

[R07] if 判断文件
来源：http://hz.ydzc1.top/gtecurhjsa.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hysaishi.cn/gtrskvwqgo.html

[R08] 数值比较
来源：http://hz.cucudq.cn/gtdxyurmjg.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.jyoumei.cn/gtbxqyobfj.html

[R09] 字符串比较
来源：http://hz.zhijiandao.cn/gteysjydjj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.tianlin.xyz/gtmohahzta.html

[R10] 正则匹配
来源：http://hz.snrcjt.cn/gtrbbvdsgn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xuetiantiany.cn/gtocyphmdl.html

[R11] case 多分支
来源：http://hz.svipenyu.cn/gtsfxsuhox.html

case "$1" in
来源：http://hz.yj202588.top/gtfarmjkuq.html

start) echo "启动" ;;
来源：http://hz.snrcjt.cn/gtfmzqgyxk.html

stop)  echo "停止" ;;
来源：http://hz.shuidangran.top/gtsiekpvnd.html

*)     echo "未知命令" ;;
来源：http://hz.yvedp.cn/gtvxqzumut.html

esac
来源：http://hz.dashuyun.cn/gtnlrhcosg.html

[R12] for 遍历文件
来源：http://hz.jyoumei.cn/gtsufejpxy.html

for f in *.txt; do echo "$f"; done
来源：http://hz.andypj.xyz/gtphvrjkvi.html

[R13] for 计数循环
来源：http://hz.zhixingplan.top/gtoorcfhyk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jyoumei.cn/gtsvbvmryv.html

[R14] C 风格 for
来源：http://hz.aibaodan.cn/gtglijjapv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sweek.top/gtrxngczgn.html

[R15] while 逐行读文件
来源：http://hz.nanxinkj.top/gtrnkzujrv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.zdqjudy.top/gtbnzvaacr.html

[R16] until 等待条件
来源：http://hz.yj20258888.top/gtqgixrfvg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.yonumen.top/gtwuyirpin.html

[R17] 数组定义与取值
来源：http://hz.xingfuxueyuan.xyz/gtpsojeasz.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtiwkmfamt.html

[R18] 遍历数组
来源：http://hz.chenzaomai.com/gteqaoyszb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.iojbl.cn/gtibvhrqax.html

[R19] 数组长度
来源：http://hz.ydjk.org.cn/gttupnoklw.html

echo "${#arr[@]}"
来源：http://hz.smart0.xyz/gtoqxytrui.html

[R20] 关联数组（字典）
来源：http://hz.nwbrower.top/gtoufjdfkr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.gzhubu.top/gtpkxnogbw.html

[R21] 字符串长度
来源：http://hz.zhongyouzk.top/gtgexhaaaj.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtsqtmdrqz.html

[R22] 截取子串
来源：http://hz.smart0.xyz/gtdhwkegsg.html

echo "${s:0:5}"
来源：http://hz.shangyingyoupin.top/gtaafehrjf.html

[R23] 字符串替换
来源：http://hz.shangyingyoupin.top/gtfjemslck.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.snrcjt.cn/gtozaotscb.html

[R24] 大小写转换
来源：http://hz.tanke756.top/gtcmnwofpr.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cheryme.top/gttlntebwk.html

[R25] 去后缀 / 去前缀
来源：http://hz.52xcode.cn/gtufgtguap.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.sysykeji.top/gtpxnstwed.html

[R26] 命令替换
来源：http://hz.birdmap.top/gtbtvaodur.html

now=$(date +%F); echo "$now"
来源：http://hz.jlsjyb.cn/gtpyilkkka.html

[R27] 算术展开
来源：http://hz.meibo888.top/gtfiddixuz.html

echo $((1 + 2 * 3))
来源：http://hz.jqgfzy.top/gtccwrvaqc.html

[R28] 浮点运算
来源：http://hz.snrcjt.cn/gtoclmqhmj.html

echo "scale=2; 10/3" | bc
来源：http://hz.jiagoushi.top/gtdruifcqv.html

[R29] 定义函数
来源：http://hz.quarkkingdee.top/gtvgcwziiv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.birdmap.top/gtuyottdcx.html

[R30] 函数返回状态码
来源：http://hz.hysaishi.cn/gtgjcswhin.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.feifeiyinyue.top/gttqlzszcn.html

[R31] 局部变量
来源：http://hz.yongpay.top/gtqxflnbgj.html

f() { local x=1; echo "$x"; }
来源：http://hz.jianghu66.top/gtfzsxjepg.html

[R32] 参数个数校验
来源：http://hz.52xcode.cn/gttuzweygu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fengsongda.top/gtacusmprb.html

[R33] 捕获错误并提示行号
来源：http://hz.pycfn.com/gtyahdvsta.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shanyushiyangtech.top/gtvuuwbndk.html

[R34] 退出时清理
来源：http://hz.dashuyun.cn/gttenuueos.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.316326.xyz/gtvrbgiuwo.html

[R35] 后台执行并等待
来源：http://hz.feifeiyinyue.top/gtujkofqzo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jlsjyb.cn/gtxdhdenmx.html

[R36] 并发执行多个任务
来源：http://hz.tianlin.xyz/gtwymoxuei.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yj20258888.top/gtjegbukdq.html

[R37] 把输出赋给变量
来源：http://hz.zhijiandao.cn/gtunxazctg.html

files=$(ls -1)
来源：http://hz.sysykeji.top/gtexwdeqqa.html

[R38] 管道串联
来源：http://hz.yangfankeji.com/gtzmuqhaae.html

cat a.txt | grep -i error | wc -l
来源：http://hz.cashguo.top/gtvbbckihg.html

[R39] 重定向标准输出与错误
来源：http://hz.aibaodan.cn/gtqygtmnbx.html

cmd > out.log 2>&1
来源：http://hz.jinghuilouyu.cn/gtvaiqcpts.html

[R40] 追加写日志
来源：http://hz.snrcjt.cn/gtlzyyeaux.html

echo "log" >> out.log
来源：http://hz.yongpay.top/gtecabsuol.html

[R41] 丢弃输出
来源：http://hz.mhx1999.top/gtnlomtuvr.html

cmd >/dev/null 2>&1
来源：http://hz.hfpthk.cn/gtntklqrec.html

[R42] 输入重定向
来源：http://hz.316326.xyz/gtztzgoqvn.html

wc -l < a.txt
来源：http://hz.hongshengwenyu.top/gtcrpndkik.html

[R43] 按名字查找文件
来源：http://hz.sysykeji.top/gtvkdtegbf.html

find . -name "*.log" -type f
来源：http://hz.yj202588.top/gtjczibbxf.html

[R44] 按修改时间查找
来源：http://hz.yvedp.cn/gtftmegprd.html

find . -mtime -7 -type f
来源：http://hz.ydjk.org.cn/gtxwytrage.html

[R45] 批量删除
来源：http://hz.pengpengdd.cyou/gttwdpkdia.html

find . -name "*.tmp" -delete
来源：http://hz.yonumen.top/gtxyuaplfw.html

[R46] 递归替换文件内容
来源：http://hz.jiagoushi.top/gtapfjrlcb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.nanxuanxn.top/gtxpjfxfbm.html

[R47] sed 单行替换
来源：http://hz.cashguo.top/gtkfsawepb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jianghu66.top/gtnefpiicu.html

[R48] awk 取指定列
来源：http://hz.gotoacloud.top/gtotsfdlri.html

awk '{print $1, $3}' a.txt
来源：http://hz.haohaochexian.top/gtoayfqxac.html

[R49] awk 带条件
来源：http://hz.xuanzx.com/gtebenzwoo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.jlsjyb.cn/gtcellpmvf.html

[R50] awk 求和
来源：http://hz.hnqzz.top/gtxnxwdwth.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.nwbrower.top/gtjgiinmbp.html

[R51] 排序去重取前几
来源：http://hz.c1oappe.top/gthxpofjad.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gogol.net.cn/gtxuzjdtjf.html

[R52] 统计行数
来源：http://hz.tian-w.cn/gtuvaoxejl.html

wc -l a.txt
来源：http://hz.fzhhl.top/gtqyywfhtv.html

[R53] 查看文件头与实时尾
来源：http://hz.xziqi.cn/gtovpimebn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ivvv.top/gtrtufwwts.html

[R54] 比较两个文件
来源：http://hz.zhongyouzk.top/gtlfkpovre.html

diff a.txt b.txt
来源：http://hz.zdqjudy.top/gtsapvnndv.html

[R55] 压缩与解压
来源：http://hz.ydjk.org.cn/gtcfkbovvf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.snrcjt.cn/gtyfwciqgq.html

[R56] 远程拷贝
来源：http://hz.shangyingyoupin.top/gtmbkqavpz.html

scp file user@host:/path/
来源：http://hz.cdnleiting.top/gthmfanhvl.html

[R57] 远程执行命令
来源：http://hz.fengsongda.top/gtbwndhsyf.html

ssh user@host 'uptime'
来源：http://hz.zhixingplan.top/gtbxgrfzed.html

[R58] 下载文件
来源：http://hz.yangfankeji.com/gtplznczrc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.tianlin.xyz/gtzhwhfimv.html

[R59] 发 POST JSON
来源：http://hz.jinyuanbaomall.cn/gtixmqfzun.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.gogol.net.cn/gtgaflszau.html

[R60] 只看 HTTP 状态码
来源：http://hz.pengpengdd.cyou/gtdsyvfjvx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yueranfly.top/gteicigygd.html

[R61] 磁盘占用
来源：http://hz.zhijiandao.cn/gthkccojeg.html

df -h;  du -sh *
来源：http://hz.hongshengwenyu.top/gthiznwarh.html

[R62] 找最占空间的文件
来源：http://hz.mhx1999.top/gtqdknsoig.html

du -ah . | sort -rh | head -10
来源：http://hz.cqqwz.cn/gttctvrsqm.html

[R63] 内存与进程
来源：http://hz.wangshuangyany.cn/gtcvmtbhaf.html

free -h;  ps aux | grep nginx
来源：http://hz.gotoacloud.top/gtjlimrdhy.html

[R64] 结束进程
来源：http://hz.ehwqpu.com/gteyprcudo.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jyoumei.cn/gtujuaarmw.html

[R65] 查看端口占用
来源：http://hz.jqgufenzy.top/gtlrdsttdg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jqgufenzy.top/gtulmboluy.html

[R66] 定时任务
来源：http://hz.fengsongda.top/gtylihlffy.html

crontab -e;  crontab -l
来源：http://hz.shzxlz.cn/gtbsuhflvx.html

[R67] 生成随机十六进制串
来源：http://hz.aibaodan.cn/gtrhkywizf.html

openssl rand -hex 16
来源：http://hz.jqgufenzy.top/gtczkytmre.html

[R68] 计算文件校验值
来源：http://hz.chenzaomai.com/gtwftypypu.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtxnlceuro.html

[R69] 生成随机密码
来源：http://hz.zhaomingkeji.xyz/gtwfuclqpk.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtarwzmjkc.html

[R70] 时间戳与互转
来源：http://hz.quarkkingdee.top/gtwcdjqdpy.html

date +%s;  date -d @1700000000
来源：http://hz.yvedp.cn/gtzhntedjz.html

[R71] 日期格式化
来源：http://hz.hongshengwenyu.top/gtiacaoimp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jianghu66.top/gtlcpoghfe.html

[R72] 等待端口就绪
来源：http://hz.yj20258888.top/gtgjsbambq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.fengsongda.top/gteoxzekzl.html

[R73] 分割大日志
来源：http://hz.sysykeji.top/gttimdrdza.html

split -l 1000 big.log part_
来源：http://hz.guannengcc.top/gtdfxuiltf.html

[R74] 批量重命名
来源：http://hz.yj20258.top/gtukuvucns.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hfpthk.cn/gtdgzzfygc.html

[R75] 导出环境变量
来源：http://hz.meibo888.top/gtsvfbclgl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.xylfe.cn/gttydyhgsr.html

[R76] 使用临时文件
来源：http://hz.chenlongwang.top/gtggtfpysj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.meibo888.top/gthqiwhfpr.html

[R77] 读取用户输入
来源：http://hz.zhijiandao.cn/gtzforxnaf.html

read -rp "请输入: " ans
来源：http://hz.sufxvd.cn/gtytnddgqn.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gtnictgdtc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.mhx1999.top/gtmytbyana.html

[R79] 解析命令行选项
来源：http://hz.jqgfzy.top/gtkikiusdm.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yuanzhike.top/gtozlwmhvy.html

[R80] 查看脚本执行耗时
来源：http://hz.yangfankeji.com/gtzplklhnp.html

time ./run.sh
来源：http://hz.xziqi.cn/gtkogfskqz.html

================================================================================
来源：http://hz.zdqjudy.top/gtkqadgrhc.html

S. C / C++ 专题
来源：http://hz.aibaodan.cn/gtgsukzfpf.html

================================================================================
来源：http://hz.pycfn.com/gtykanwksa.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtjnleweoo.html

#include <stdio.h>
来源：http://hz.zhengqikj.top/gtvhwgngfw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xylfe.cn/gtlraancbh.html

[S02] C：变量与格式化输出
来源：http://hz.ydzc1.top/gtyvicmqow.html

int a = 10; printf("%d\n", a);
来源：http://hz.0kj1m.cn/gtoepblvhp.html

[S03] C：读入整数
来源：http://hz.daria6918.cn/gtwjruonbg.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gtpavfayxs.html

[S04] C：字符串复制
来源：http://hz.zdqjudy.top/gtxwwlxsuq.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.haohaochexian.top/gtvecyuxuk.html

[S05] C：字符串长度
来源：http://hz.mhx1999.top/gtihiyidtd.html

strlen(s)
来源：http://hz.haohaochexian.top/gtdizayucu.html

[S06] C：字符串比较
来源：http://hz.fengsongda.top/gtlupnkhhu.html

strcmp(a, b) == 0
来源：http://hz.yj20258888.top/gtumfhkxeh.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtnzdkilff.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.sufxvd.cn/gtofmstfgz.html

[S08] C：动态内存分配与释放
来源：http://hz.bjfxy.top/gtercbrfla.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.ydjk.org.cn/gtyvfkdvnx.html

[S09] C：结构体定义与初始化
来源：http://hz.nanxinkj.top/gtabytlcam.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.c1oappe.top/gtnbczvixz.html

[S10] C：指针与解引用
来源：http://hz.cashguo.top/gtojmemwqu.html

int *p = &a;  *p = 5;
来源：http://hz.shangyingyoupin.top/gtxqdebbyf.html

[S11] C：逐行读文件
来源：http://hz.yuxming.cn/gtuuhlwakm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.iojbl.cn/gtoznxkhxn.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.mhx1999.top/gtcgtjetse.html

fclose(f);
来源：http://hz.gotoacloud.top/gtqvzetime.html

[S12] C：写文件
来源：http://hz.cucudq.cn/gtwbgdaylh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ybcxt.top/gtfwbwuecs.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gtrpyufvah.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.andypj.xyz/gtbijdpscc.html

[S14] C：枚举
来源：http://hz.gotoacloud.top/gtjnuvhuzr.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sysykeji.top/gtvebcrtev.html

[S15] C：类型转换
来源：http://hz.cdnleiting.top/gtmrtryogf.html

(double) a / b
来源：http://hz.c1oappe.top/gtgutcpiaz.html

[S16] C：位操作置位
来源：http://hz.zhaomingkeji.xyz/gtcnzzqtdx.html

x |= (1 << 3);
来源：http://hz.cqqwz.cn/gtrmxenwrr.html

[S17] C：安全拼接字符串
来源：http://hz.yanxiufei.cn/gtljfsqjlr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.zdqjudy.top/gtepovzpxa.html

[S18] C：命令行参数
来源：http://hz.iojbl.cn/gturuuhllt.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gttkdjvptb.html

[S19] C：快速排序
来源：http://hz.jinyuanbaomall.cn/gtaqczfqja.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yonumen.top/gtwwfghyeg.html

[S20] C：二分查找
来源：http://hz.zhongyouzk.top/gtxwvxjfem.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.jinyuanbaomall.cn/gtmweuukns.html

[S21] C：字符类别判断
来源：http://hz.yuxming.cn/gtlrkxtkhw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shuidangran.top/gttrnbmwjf.html

[S22] C：字符串转数字
来源：http://hz.9152youxi.cn/gtusnkclpc.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.chenlongwang.top/gtgmcgizwt.html

[S23] C：随机数
来源：http://hz.jqgufenzy.top/gtfjzqulfp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sufxvd.cn/gturhdzlty.html

[S24] C：获取本地时间
来源：http://hz.shanyushiyangtech.top/gtbdtbgkax.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.feifeiyinyue.top/gthwgtkjxf.html

[S25] C：内存拷贝
来源：http://hz.yanxiufei.cn/gtqhxibodh.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtnmjvzdhu.html

[S26] C：内存清零
来源：http://hz.jinqigfzy.top/gtlfamkghl.html

memset(a, 0, sizeof a);
来源：http://hz.sweek.top/gtdjuvcjpm.html

[S27] C：定义常量
来源：http://hz.ywan-chungtsiang.top/gtrzzwdrqy.html

const double PI = 3.14159;
来源：http://hz.ywan-chungtsiang.top/gtztedqgjv.html

[S28] C：静态变量
来源：http://hz.chenzaomai.com/gtltaymfzh.html

static int counter = 0;
来源：http://hz.quarkkingdee.top/gtlvjcoenc.html

[S29] C：变参函数
来源：http://hz.xuanzx.com/gtbxlarhvc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.yangfankeji.com/gtbuuzbvle.html

[S30] C：头文件保护
来源：http://hz.kuanghao11.cn/gtialomemj.html

#ifndef X_H
来源：http://hz.zycfv.cn/gtiilkebvz.html

#define X_H
来源：http://hz.hnxiangtu.top/gtywlcejxu.html

#endif
来源：http://hz.yueranfly.top/gtwwmtgqto.html

[S31] C++：Hello World
来源：http://hz.sweek.top/gtxbyahqpi.html

#include <iostream>
来源：http://hz.smart0.xyz/gtraopezah.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.kuanghao11.cn/gtvppnnmod.html

[S32] C++：字符串
来源：http://hz.jinghuilouyu.cn/gtteqyggit.html

std::string s = "hi";  s += "!";
来源：http://hz.wangshuangyany.cn/gtttioyxry.html

[S33] C++：vector 增删
来源：http://hz.ybcxt.top/gtoshcpfhn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.zhaomingkeji.xyz/gtjecuhcod.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtmgjjsjwy.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.chenjidiqi.icu/gttaayluyk.html

[S35] C++：map
来源：http://hz.cucudq.cn/gtiftfoqhe.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtneqpynfw.html

[S36] C++：unordered_map
来源：http://hz.xuetiantiany.cn/gtxichoxpg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jiagoushi.top/gtslauvyta.html

[S37] C++：set
来源：http://hz.yangfankeji.com/gtzqqjioxm.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sweek.top/gtpryywekf.html

[S38] C++：排序
来源：http://hz.ydjk.org.cn/gtqwmnttha.html

std::sort(v.begin(), v.end());
来源：http://hz.ywan-chungtsiang.top/gtewlcvzoy.html

[S39] C++：自定义比较器排序
来源：http://hz.yangfankeji.com/gtgkxmckkt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.guannengcc.top/gtmvyessqc.html

[S40] C++：查找元素
来源：http://hz.meibo888.top/gtpnsimjlc.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.316326.xyz/gtfngojwqu.html

[S41] C++：类与构造函数
来源：http://hz.0kj1m.cn/gthgpjuhfg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.birdmap.top/gtchclbexy.html

[S42] C++：继承与虚函数
来源：http://hz.andypj.xyz/gtfttkjuzn.html

class B : public Base { public: void f() override {} };
来源：http://hz.shangyingyoupin.top/gtpraaekxk.html

[S43] C++：智能指针
来源：http://hz.ehwqpu.com/gternbviij.html

auto p = std::make_unique<int>(5);
来源：http://hz.nanxinkj.top/gtyssiymab.html

[S44] C++：引用传参
来源：http://hz.hnqzz.top/gtjwadzsrl.html

void inc(int &x) { ++x; }
来源：http://hz.xuanzx.com/gtwmvkyxpt.html

[S45] C++：lambda
来源：http://hz.zdqjudy.top/gtqvkqacjs.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.haohaochexian.top/gtwzbcedgr.html

[S46] C++：函数模板
来源：http://hz.zhixingplan.top/gthnbyffgm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.chenlongwang.top/gtwwckztck.html

[S47] C++：结构化绑定遍历
来源：http://hz.sweek.top/gtbfpkgtxq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xylfe.cn/gtjvpmjcmg.html

[S48] C++：逐行读文件
来源：http://hz.nanxinkj.top/gtngjysxhm.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.pengpengdd.cyou/gtzbekdyqi.html

while (std::getline(in, line)) { }
来源：http://hz.52xcode.cn/gtiiattfqs.html

[S49] C++：写文件
来源：http://hz.xziqi.cn/gtjxysrfgx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.hfpthk.cn/gtinlijeyd.html

[S50] C++：格式化数字
来源：http://hz.yangfankeji.com/gtkrxyohxp.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.shzxlz.cn/gtwvoajajz.html

[S51] C++：显式类型转换
来源：http://hz.sxryk.cn/gtmqiluuyb.html

static_cast<double>(a) / b
来源：http://hz.yangfankeji.com/gtlzrliwnp.html

[S52] C++：const 与 noexcept
来源：http://hz.jlsjyb.cn/gtvetmoias.html

int size() const noexcept { return n_; }
来源：http://hz.chenjidiqi.icu/gthnxohxbp.html

[S53] C++：移动语义
来源：http://hz.aizwys.cn/gtzcjvubku.html

std::vector<int> w = std::move(v);
来源：http://hz.sweek.top/gtrahkieot.html

[S54] C++：异常处理
来源：http://hz.jyoumei.cn/gtwjxamnyf.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.fzhhl.top/gtqhqrvehe.html

[S55] C++：结构化绑定
来源：http://hz.jianghu66.top/gtqwmroszy.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.jinyuanbaomall.cn/gtyaykbsxf.html

[S56] C++：optional
来源：http://hz.guannengcc.top/gtevftcjvg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.fengsongda.top/gtninggcdc.html

[S57] C++：编译期常量
来源：http://hz.hysaishi.cn/gtnnqyhvbt.html

constexpr int N = 10;
来源：http://hz.quarkkingdee.top/gtoqbdnocr.html

[S58] C++：命名空间
来源：http://hz.yj20258.top/gtikogmoav.html

namespace ns { int f() { return 1; } }
来源：http://hz.quarkkingdee.top/gtdzcvgaja.html

[S59] C++：静态断言
来源：http://hz.xylfe.cn/gtijatuhvc.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.yuanzhike.top/gtinplpkmv.html

[S60] C++：遍历并删除元素
来源：http://hz.sysykeji.top/gtyhzljuni.html


<!-- 参考信息 -->