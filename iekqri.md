代发 wailian999

case "$1" in
来源：http://hz.dashuyun.cn/gtkljzgomy.html

start) echo "启动" ;;
来源：http://hz.hnxiangtu.top/gtiazzscaq.html

stop)  echo "停止" ;;
来源：http://hz.ydzc1.top/gtbklgofhf.html

*)     echo "未知命令" ;;
来源：http://hz.shanyushiyangkeji.top/gtpprknmdz.html

esac
来源：http://hz.52xcode.cn/gtuwrvtpvr.html

[R12] for 遍历文件
来源：http://hz.haohaochexian.top/gtlbpvkwby.html

for f in *.txt; do echo "$f"; done
来源：http://hz.sxryk.cn/gtomlpetol.html

[R13] for 计数循环
来源：http://hz.zhixingplan.top/gtlfhrlnwg.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.bjfxy.top/gtxmvdmtsz.html

[R14] C 风格 for
来源：http://hz.yj202588.top/gtcynnrotc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.sysykeji.top/gtihzgyaac.html

[R15] while 逐行读文件
来源：http://hz.yanxiufei.cn/gtnaymcbqn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yonumen.top/gtdbdpadea.html

[R16] until 等待条件
来源：http://hz.zhiwuduotai.top/gtxzyfvrjl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.chenlongwang.top/gtteuhqqcs.html

[R17] 数组定义与取值
来源：http://hz.jinqigfzy.top/gtvjuxjpye.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cdnleiting.top/gtrwerwbnd.html

[R18] 遍历数组
来源：http://hz.birdmap.top/gtcgblrlck.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtyptbqhbh.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gttmgvsfep.html

echo "${#arr[@]}"
来源：http://hz.aizwys.cn/gtpmyftijs.html

[R20] 关联数组（字典）
来源：http://hz.yj20258888.top/gtbocallzy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jlsjyb.cn/gttvmmcfur.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtqyyuuijz.html

echo "${#s}"
来源：http://hz.chenzaomai.com/gtmpqggmtb.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtnyfhupbq.html

echo "${s:0:5}"
来源：http://hz.hongshengwenyu.top/gtqfvasasq.html

[R23] 字符串替换
来源：http://hz.nanxuanxn.top/gtefwntyuq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ydzc1.top/gtovskniyg.html

[R24] 大小写转换
来源：http://hz.yj202588.top/gtspswigzy.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtbctlosaj.html

[R25] 去后缀 / 去前缀
来源：http://hz.sufxvd.cn/gthxqpcifh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.kuanghao11.cn/gtsineeglg.html

[R26] 命令替换
来源：http://hz.gaohongyu789.top/gtoayiqqgd.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgufenzy.top/gtshcxeskd.html

[R27] 算术展开
来源：http://hz.feifeiyinyue.top/gttfnowvpz.html

echo $((1 + 2 * 3))
来源：http://hz.chenjidiqi.icu/gtglynmcrm.html

[R28] 浮点运算
来源：http://hz.zhaomingkeji.xyz/gtnuqgsomy.html

echo "scale=2; 10/3" | bc
来源：http://hz.tanke756.top/gtpimmxyfu.html

[R29] 定义函数
来源：http://hz.zhaomingkeji.xyz/gteatwagxg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tianlin.xyz/gtwpadliih.html

[R30] 函数返回状态码
来源：http://hz.guannengcc.top/gtcbpyzuzh.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.wangdashe.top/gtuicphylr.html

[R31] 局部变量
来源：http://hz.ydjk.org.cn/gthuqvutjh.html

f() { local x=1; echo "$x"; }
来源：http://hz.svipenyu.cn/gtknqclvac.html

[R32] 参数个数校验
来源：http://hz.daria6918.cn/gtugutewao.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.dianchejie.cn/gtkmycptwp.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gtyiyusvqp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.mhx1999.top/gtfozrziqv.html

[R34] 退出时清理
来源：http://hz.birdmap.top/gtbfagubhs.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtpnqnmozl.html

[R35] 后台执行并等待
来源：http://hz.yonumen.top/gtnftjjbvr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hywenlv.cn/gtoygmlxac.html

[R36] 并发执行多个任务
来源：http://hz.ywan-chungtsiang.top/gtucqrbvum.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.jlsjyb.cn/gtiznxvewj.html

[R37] 把输出赋给变量
来源：http://hz.tanke756.top/gtmyvobqsh.html

files=$(ls -1)
来源：http://hz.yongpay.top/gtrcsmlnyo.html

[R38] 管道串联
来源：http://hz.sysykeji.top/gtvtxsjton.html

cat a.txt | grep -i error | wc -l
来源：http://hz.svipenyu.cn/gtwbxmvdwr.html

[R39] 重定向标准输出与错误
来源：http://hz.yongpay.top/gtuihqfmkv.html

cmd > out.log 2>&1
来源：http://hz.316326.xyz/gtzjeuyjbg.html

[R40] 追加写日志
来源：http://hz.sysykeji.top/gtftnxjuje.html

echo "log" >> out.log
来源：http://hz.jyoumei.cn/gtfgtzdbhu.html

[R41] 丢弃输出
来源：http://hz.9152youxi.cn/gtzsdmskyx.html

cmd >/dev/null 2>&1
来源：http://hz.ywan-chungtsiang.top/gtoxfupruu.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtczaakddf.html

wc -l < a.txt
来源：http://hz.yuxming.cn/gtsgprvlop.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gtohhetces.html

find . -name "*.log" -type f
来源：http://hz.cashguo.top/gtyhriimfi.html

[R44] 按修改时间查找
来源：http://hz.shuidangran.top/gtvjbgwnqv.html

find . -mtime -7 -type f
来源：http://hz.zhixingplan.top/gtipqtxivl.html

[R45] 批量删除
来源：http://hz.cucudq.cn/gtgqbfsrgm.html

find . -name "*.tmp" -delete
来源：http://hz.tianlin.xyz/gtxuiemkbw.html

[R46] 递归替换文件内容
来源：http://hz.jinghuilouyu.cn/gtxxdisyus.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yanxiufei.cn/gtxvfwljir.html

[R47] sed 单行替换
来源：http://hz.jlsjyb.cn/gtfpaayqpb.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jiagoushi.top/gtmccscrto.html

[R48] awk 取指定列
来源：http://hz.tianlin.xyz/gtlymftycw.html

awk '{print $1, $3}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtjzwekntf.html

[R49] awk 带条件
来源：http://hz.zycfv.cn/gtvfsinaeq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.dianchejie.cn/gtxtupfyxw.html

[R50] awk 求和
来源：http://hz.zhengqikj.top/gtjkrcgsof.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhaomingkeji.xyz/gtwnrrojlh.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtwfyhiqvg.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.zhengqikj.top/gtkaiwjvci.html

[R52] 统计行数
来源：http://hz.fengsongda.top/gteuamipwi.html

wc -l a.txt
来源：http://hz.cqqwz.cn/gttfxbfiua.html

[R53] 查看文件头与实时尾
来源：http://hz.gogol.net.cn/gtjakwsgfu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinqigfzy.top/gtudxmxsub.html

[R54] 比较两个文件
来源：http://hz.ywan-chungtsiang.top/gtiqawljaa.html

diff a.txt b.txt
来源：http://hz.jinyuanbaomall.cn/gtikmaonmz.html

[R55] 压缩与解压
来源：http://hz.ydjk.org.cn/gtkyfhrljr.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.wangshuangyany.cn/gtrxlrgpxb.html

[R56] 远程拷贝
来源：http://hz.jqgufenzy.top/gtxlurgrjn.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtoywnfzyh.html

[R57] 远程执行命令
来源：http://hz.ppjwa.cn/gtvuvmsaln.html

ssh user@host 'uptime'
来源：http://hz.aizwys.cn/gtazggywlf.html

[R58] 下载文件
来源：http://hz.ppjwa.cn/gtmtmfajlv.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.sweek.top/gtinbyljsg.html

[R59] 发 POST JSON
来源：http://hz.svipenyu.cn/gtclmzdosa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hongshengwenyu.top/gtskdqjpaf.html

[R60] 只看 HTTP 状态码
来源：http://hz.iojbl.cn/gtwbbdxzhq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.nanxinkj.top/gttckvejwa.html

[R61] 磁盘占用
来源：http://hz.shuidangran.top/gtyhpwgypu.html

df -h;  du -sh *
来源：http://hz.ywan-chungtsiang.top/gtwyxdimlw.html

[R62] 找最占空间的文件
来源：http://hz.shuidangran.top/gtueneiqie.html

du -ah . | sort -rh | head -10
来源：http://hz.redwolf501.top/gtbavovkdq.html

[R63] 内存与进程
来源：http://hz.shangyingyoupin.top/gtapluistm.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgfzy.top/gtnwnrtmuh.html

[R64] 结束进程
来源：http://hz.yj20258888.top/gtsimovxqm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.hammf.cn/gtfodkejms.html

[R65] 查看端口占用
来源：http://hz.shanyushiyangtech.top/gtsgfbuxxg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shanyushiyangkeji.top/gtyxqlvteh.html

[R66] 定时任务
来源：http://hz.xuetiantiany.cn/gtdiuutxng.html

crontab -e;  crontab -l
来源：http://hz.pengpengdd.cyou/gtcaqbjzkg.html

[R67] 生成随机十六进制串
来源：http://hz.gogol.net.cn/gtlwbztcat.html

openssl rand -hex 16
来源：http://hz.pengpengdd.cyou/gtesjtimqp.html

[R68] 计算文件校验值
来源：http://hz.jianghu66.top/gtmxxikpiz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cqqwz.cn/gtxdjlwqkc.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gtgzyyxzab.html

head -c 16 /dev/urandom | base64
来源：http://hz.hnxiangtu.top/gtkhwnmhlm.html

[R70] 时间戳与互转
来源：http://hz.xylfe.cn/gtjnnamnie.html

date +%s;  date -d @1700000000
来源：http://hz.andypj.xyz/gtdbpcnptt.html

[R71] 日期格式化
来源：http://hz.hammf.cn/gtjdjgdwnj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yonumen.top/gtzrwdhcym.html

[R72] 等待端口就绪
来源：http://hz.jyoumei.cn/gtuaezhkuv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.hysaishi.cn/gtnbbhpsat.html

[R73] 分割大日志
来源：http://hz.feifeiyinyue.top/gtlzurnvzz.html

split -l 1000 big.log part_
来源：http://hz.sufxvd.cn/gtmsgbzefw.html

[R74] 批量重命名
来源：http://hz.nanxinkj.top/gtdrgsaene.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.havefunace.top/gtglplqnte.html

[R75] 导出环境变量
来源：http://hz.hywenlv.cn/gtmwjwohsp.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hammf.cn/gtqbxsqeum.html

[R76] 使用临时文件
来源：http://hz.sysykeji.top/gtiwtqyrgl.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.bjfxy.top/gtwijadfrd.html

[R77] 读取用户输入
来源：http://hz.gzhubu.top/gtfvvwpmln.html

read -rp "请输入: " ans
来源：http://hz.shzxlz.cn/gtnmvykmzl.html

[R78] 交互式菜单
来源：http://hz.feifeiyinyue.top/gtuwvjsfbf.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ehwqpu.com/gtfxnfabxv.html

[R79] 解析命令行选项
来源：http://hz.yanxiufei.cn/gtrpbmncky.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.smart0.xyz/gtyodjexxd.html

[R80] 查看脚本执行耗时
来源：http://hz.snrcjt.cn/gtyvtsfwyl.html

time ./run.sh
来源：http://hz.shzxlz.cn/gtybvmqpsz.html

================================================================================
来源：http://hz.dianchejie.cn/gtetwlctlw.html

S. C / C++ 专题
来源：http://hz.yj20258.top/gtxxbbyqvc.html

================================================================================
来源：http://hz.zhijiandao.cn/gtkzblivda.html

[S01] C：Hello World
来源：http://hz.shuidangran.top/gtbhwkhtin.html

#include <stdio.h>
来源：http://hz.tianlin.xyz/gtohrxrqgb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.ehwqpu.com/gtfkkwnoyl.html

[S02] C：变量与格式化输出
来源：http://hz.yj20258888.top/gtiphbztiz.html

int a = 10; printf("%d\n", a);
来源：http://hz.jinqigfzy.top/gtoooyxlcl.html

[S03] C：读入整数
来源：http://hz.hywenlv.cn/gtmlrypcab.html

int x; scanf("%d", &x);
来源：http://hz.pycfn.com/gtsvppnoab.html

[S04] C：字符串复制
来源：http://hz.yueranfly.top/gtfohwkanb.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ivvv.top/gtopnevdam.html

[S05] C：字符串长度
来源：http://hz.hfpthk.cn/gtsbuqzefk.html

strlen(s)
来源：http://hz.jiagoushi.top/gtakjqnpha.html

[S06] C：字符串比较
来源：http://hz.tian-w.cn/gtctrxwbrd.html

strcmp(a, b) == 0
来源：http://hz.zhoulong.xyz/gtkrtitwyj.html

[S07] C：数组遍历求和
来源：http://hz.jinqigfzy.top/gtvqjfaiwa.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ydzc1.top/gtfoinyfcn.html

[S08] C：动态内存分配与释放
来源：http://hz.0kj1m.cn/gtqerqsmyz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jlsjyb.cn/gtuornnohw.html

[S09] C：结构体定义与初始化
来源：http://hz.jyoumei.cn/gtdzdzryjo.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.tian-w.cn/gtsuplohih.html

[S10] C：指针与解引用
来源：http://hz.feifeiyinyue.top/gthbsjpmhz.html

int *p = &a;  *p = 5;
来源：http://hz.zhixingplan.top/gtppufmphg.html

[S11] C：逐行读文件
来源：http://hz.snrcjt.cn/gtrahmrtdm.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jianghu66.top/gtsvdcnhsv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.aizwys.cn/gtxfozyprk.html

fclose(f);
来源：http://hz.pengpengdd.cyou/gtcsiaaloj.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtachppbjm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gogol.net.cn/gtkfypcrum.html

[S13] C：宏定义
来源：http://hz.316326.xyz/gtdcwpvhbg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtldatrmxw.html

[S14] C：枚举
来源：http://hz.tanke756.top/gtszxkcegx.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.birdmap.top/gtuxptpvjk.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtejwxqcyg.html

(double) a / b
来源：http://hz.dashuyun.cn/gtkteucasw.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtrwqjgrsb.html

x |= (1 << 3);
来源：http://hz.vqdsnc.cn/gtmmbjfqgt.html

[S17] C：安全拼接字符串
来源：http://hz.guowangkeji.top/gtkebuaofq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.shzxlz.cn/gtbllxdszh.html

[S18] C：命令行参数
来源：http://hz.zhongyouzk.top/gttxmeuwjl.html

int main(int argc, char **argv)
来源：http://hz.zhongyouzk.top/gtnwbkgzhn.html

[S19] C：快速排序
来源：http://hz.cheryme.top/gtglnffwtc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtbsjwtstz.html

[S20] C：二分查找
来源：http://hz.pengpengdd.cyou/gthhtpjpcz.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shanyushiyangtech.top/gtjkgxzeey.html

[S21] C：字符类别判断
来源：http://hz.zhixingplan.top/gtesunwfwu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xinyue.icu/gtqgvjuwax.html

[S22] C：字符串转数字
来源：http://hz.jinyuanbaomall.cn/gtybaxbzxu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.tanke756.top/gtidkjwety.html

[S23] C：随机数
来源：http://hz.dianchejie.cn/gtsprgivwn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cdnleiting.top/gtkaagczpt.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtbqooqkio.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.shanyushiyangtech.top/gtgrsmhaqb.html

[S25] C：内存拷贝
来源：http://hz.52xcode.cn/gtoqptnvbd.html

memcpy(dst, src, n);
来源：http://hz.jqgufenzy.top/gtgfnmylax.html

[S26] C：内存清零
来源：http://hz.hnxiangtu.top/gtonefrpmz.html

memset(a, 0, sizeof a);
来源：http://hz.zhongyouzk.top/gtuzctnluv.html

[S27] C：定义常量
来源：http://hz.hysaishi.cn/gtgshpkgni.html

const double PI = 3.14159;
来源：http://hz.hysaishi.cn/gtrajpaept.html

[S28] C：静态变量
来源：http://hz.yj202588.top/gtkfwilupr.html

static int counter = 0;
来源：http://hz.yuanzhike.top/gtbtwpdxrd.html

[S29] C：变参函数
来源：http://hz.yueranfly.top/gtbcqznaqz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.birdmap.top/gtzobbrdra.html

[S30] C：头文件保护
来源：http://hz.jqgufenzy.top/gtbvzolmzp.html

#ifndef X_H
来源：http://hz.hywenlv.cn/gtuewmkvsb.html

#define X_H
来源：http://hz.zhongyouzk.top/gtyndcibbw.html

#endif
来源：http://hz.cashguo.top/gtujpmihde.html

[S31] C++：Hello World
来源：http://hz.iojbl.cn/gtnichszes.html

#include <iostream>
来源：http://hz.hnxiangtu.top/gtdjparrgf.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.cashguo.top/gtlgskcrtm.html

[S32] C++：字符串
来源：http://hz.yangfankeji.com/gtkfphhbwc.html

std::string s = "hi";  s += "!";
来源：http://hz.tian-w.cn/gtxrjkqdcv.html

[S33] C++：vector 增删
来源：http://hz.ppjwa.cn/gtaldmidts.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cashguo.top/gtfcwtoywk.html

[S34] C++：遍历 vector
来源：http://hz.hywenlv.cn/gtszzsxwiv.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.vqdsnc.cn/gtomeovcfl.html

[S35] C++：map
来源：http://hz.hysaishi.cn/gtxqkdhdfb.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.jinyuanbaomall.cn/gtvsnskgxy.html

[S36] C++：unordered_map
来源：http://hz.yueranfly.top/gtuwrtdrbm.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ivvv.top/gtcckaskdh.html

[S37] C++：set
来源：http://hz.guowangkeji.top/gtjgwjiuln.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.smart0.xyz/gtlpcqtpuu.html

[S38] C++：排序
来源：http://hz.fengsongda.top/gtbcesrjxo.html

std::sort(v.begin(), v.end());
来源：http://hz.hnxiangtu.top/gtnbmumrzp.html

[S39] C++：自定义比较器排序
来源：http://hz.yj202588.top/gtdfeocabl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.zhijiandao.cn/gtmutkeiwd.html

[S40] C++：查找元素
来源：http://hz.fengsongda.top/gtsfapwflb.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.xingfuxueyuan.xyz/gtdchqeoxm.html

[S41] C++：类与构造函数
来源：http://hz.chenjidiqi.icu/gtpyagmvvc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.sxryk.cn/gtkfrqandr.html

[S42] C++：继承与虚函数
来源：http://hz.cqqwz.cn/gtqthladed.html

class B : public Base { public: void f() override {} };
来源：http://hz.chenlongwang.top/gtohpxlusr.html

[S43] C++：智能指针
来源：http://hz.quarkkingdee.top/gthohsdnjm.html

auto p = std::make_unique<int>(5);
来源：http://hz.zdqjudy.top/gtzbugnmbr.html

[S44] C++：引用传参
来源：http://hz.jlsjyb.cn/gtduxebbcp.html

void inc(int &x) { ++x; }
来源：http://hz.hfpthk.cn/gttuhvzbhk.html

[S45] C++：lambda
来源：http://hz.ivvv.top/gtafbxqgcj.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.yangfankeji.com/gtxdnygatr.html

[S46] C++：函数模板
来源：http://hz.nanxuanxn.top/gtryzfcphw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zdqjudy.top/gtsrqqnmai.html

[S47] C++：结构化绑定遍历
来源：http://hz.316326.xyz/gtpkdixzjl.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.xuetiantiany.cn/gttowsolby.html

[S48] C++：逐行读文件
来源：http://hz.xuetiantiany.cn/gtnlmvchgo.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.nanxinkj.top/gtwxjbprdh.html

while (std::getline(in, line)) { }
来源：http://hz.yj202588.top/gtgdkwqeem.html

[S49] C++：写文件
来源：http://hz.jianghu66.top/gtsubkxhob.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.chenlongwang.top/gtaztjgter.html

[S50] C++：格式化数字
来源：http://hz.haohaochexian.top/gtwpvtfegd.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.hnqzz.top/gtffqqayxq.html

[S51] C++：显式类型转换
来源：http://hz.nanxinkj.top/gtutdunhpt.html

static_cast<double>(a) / b
来源：http://hz.zhijiandao.cn/gtxtcfrpdq.html

[S52] C++：const 与 noexcept
来源：http://hz.xuanzx.com/gtbedsrhoe.html

int size() const noexcept { return n_; }
来源：http://hz.aizwys.cn/gttrvrdrju.html

[S53] C++：移动语义
来源：http://hz.cqqwz.cn/gtfckmfbqf.html

std::vector<int> w = std::move(v);
来源：http://hz.smart0.xyz/gtrthjlytq.html

[S54] C++：异常处理
来源：http://hz.chenlongwang.top/gttciqljai.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hz.wangdashe.top/gtizzmisbr.html

[S55] C++：结构化绑定
来源：http://hz.fengsongda.top/gtnzwtqlms.html

auto [a, b] = std::make_pair(1, 2);
来源：http://hz.ivvv.top/gtiywhrrqn.html

[S56] C++：optional
来源：http://hz.shangyingyoupin.top/gtzzdwvopz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hz.bjfxy.top/gtbrfsxmls.html

[S57] C++：编译期常量
来源：http://hz.hnxiangtu.top/gtmchdsfqa.html

constexpr int N = 10;
来源：http://hz.tianlin.xyz/gtyifmnoxj.html

[S58] C++：命名空间
来源：http://hz.guowangkeji.top/gtyrynhenx.html

namespace ns { int f() { return 1; } }
来源：http://hz.cqqwz.cn/gtnrlkhofq.html

[S59] C++：静态断言
来源：http://hz.nanxuanxn.top/gttxiuaoar.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hz.zhaomingkeji.xyz/gtnvszfwsm.html

[S60] C++：遍历并删除元素
来源：http://hz.fengsongda.top/gtustekvno.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hz.wangshuangyany.cn/gtrdandvhp.html

================================================================================
来源：http://hz.ehwqpu.com/gtfctgphng.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hz.dianchejie.cn/gtjopvqvfs.html

================================================================================
来源：http://hz.hnxiangtu.top/gthqmkltbu.html

[T01] Kotlin：Hello World
来源：http://hz.gaohongyu789.top/gtjacvnzps.html

println("Hello")
来源：http://hz.jinqigufen.top/gtibsagdav.html

[T02] Kotlin：变量
来源：http://hz.sysykeji.top/gtrqnptild.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hz.dashuyun.cn/gtjkiwpmix.html

[T03] Kotlin：字符串模板
来源：http://hz.jianghu66.top/gtgchcktgf.html

"值: $b"
来源：http://hz.smart0.xyz/gtzaumofec.html

[T04] Kotlin：空安全
来源：http://hz.birdmap.top/gtampuavcy.html

val n: String? = null;  n?.length
来源：http://hz.yuanzhike.top/gthaoehsxk.html

[T05] Kotlin：when 表达式
来源：http://hz.9152youxi.cn/gteediqcma.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.yanxiufei.cn/gtjwbwnyqn.html

[T06] Kotlin：集合映射
来源：http://hz.zhongyouzk.top/gtffsigoxl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://hz.yvedp.cn/gttwacgrvg.html

[T07] Kotlin：集合过滤
来源：http://hz.yj20258.top/gtjisysjnu.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://hz.ppjwa.cn/gtzxvrnhfi.html

[T08] Kotlin：数据类
来源：http://hz.jinyuanbaomall.cn/gtcnhxynbi.html

data class User(val name: String, val age: Int)
来源：http://hz.52xcode.cn/gtatwabbyn.html

[T09] Kotlin：扩展函数
来源：http://hz.daria6918.cn/gtcqmgsgmp.html

fun String.exclaim() = this + "!"
来源：http://hz.zhijiandao.cn/gtxoqcwksk.html

[T10] Kotlin：默认参数
来源：http://hz.zhaomingkeji.xyz/gtwkbivhrp.html

fun greet(name: String = "World") = "Hi $name"
来源：http://hz.jqgfzy.top/gtgpfikloh.html

[T11] Kotlin：协程
来源：http://hz.shangyingyoupin.top/gtyzfvlnll.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://hz.snrcjt.cn/gtzysvqaul.html

[T12] Kotlin：解构声明
来源：http://hz.ivvv.top/gtbcpbqhou.html

val (a, b) = Pair(1, 2)
来源：http://hz.316326.xyz/gtkvdeixax.html


<!-- 参考信息 -->