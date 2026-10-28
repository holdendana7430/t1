代发 wailian999

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtfnudsgki.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.bjfxy.top/gtyhrhgjkn.html

[Q79] 字符串拼接
来源：http://hz.nanxuanxn.top/gtbfdpeigs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tianlin.xyz/gtffdqvluu.html

[Q80] 字符串截取
来源：http://hz.jinghuilouyu.cn/gtgsyemxob.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.c1oappe.top/gttpaaitrw.html

[Q81] 字符串替换
来源：http://hz.nanxuanxn.top/gtpkzfafzb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hnxiangtu.top/gtjxeqcxwq.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtuvwxgdwu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.andypj.xyz/gtiimllkxz.html

[Q83] 大小写转换
来源：http://hz.sweek.top/gtbwzmkpkn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.svipenyu.cn/gtzjgvfljr.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gtnqkvyzho.html

SELECT TRIM(name) FROM users;
来源：http://hz.yueranfly.top/gtnhhsgljc.html

[Q85] 数值取整
来源：http://hz.nwbrower.top/gtjqvqarkl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinyuanbaomall.cn/gthkgrejtk.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gtsodfizch.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sweek.top/gtsomofuko.html

[Q87] JSON 字段做条件
来源：http://hz.zycfv.cn/gtkwpqczwh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.tanke756.top/gtnwaiessh.html

[Q88] 行转列（条件聚合）
来源：http://hz.hywenlv.cn/gtrfarkuam.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtedrkclzx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sxryk.cn/gtzwocgwok.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtltvnqocu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.wangdashe.top/gtxpfrglvg.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtmfqoeqtc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.jinyuanbaomall.cn/gteedpqosg.html

================================================================================
来源：http://hz.bjfxy.top/gtzttpmwah.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtoflfshlj.html

================================================================================
来源：http://hz.jqgufenzy.top/gtwnijmiqu.html

[R01] shebang 与严格模式
来源：http://hz.ydzc1.top/gtljidccjn.html

#!/usr/bin/env bash
来源：http://hz.nanxinkj.top/gtfzjojrmj.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtqnwvlojd.html

[R02] 变量赋值与使用
来源：http://hz.chenlongwang.top/gtqqbaftpl.html

name="Tom"; echo "$name"
来源：http://hz.cheryme.top/gtegkmdxob.html

[R03] 只读变量
来源：http://hz.zhengqikj.top/gtldawrcfb.html

readonly PI=3.14
来源：http://hz.gogol.net.cn/gtasuevaen.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtpcpnqgfm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtsfnhqmld.html

[R05] 参数默认值
来源：http://hz.sysykeji.top/gtcplvshte.html

name="${1:-default}"
来源：http://hz.daria6918.cn/gtpdfmxhxc.html

[R06] 判断命令是否存在
来源：http://hz.tian-w.cn/gtzsusrwzs.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yueranfly.top/gtavwqcfgv.html

[R07] if 判断文件
来源：http://hz.sxryk.cn/gtpotthoop.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guowangkeji.top/gthzfoemna.html

[R08] 数值比较
来源：http://hz.chenjidiqi.icu/gttkoylggc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.shanyushiyangkeji.top/gtzztqsrkp.html

[R09] 字符串比较
来源：http://hz.ydjk.org.cn/gtyvdnzvda.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.havefunace.top/gtnjiaifgg.html

[R10] 正则匹配
来源：http://hz.zycfv.cn/gtftbmukso.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.kuanghao11.cn/gtvhkpapsy.html

[R11] case 多分支
来源：http://hz.quarkkingdee.top/gtgjzvsdcr.html

case "$1" in
来源：http://hz.cucudq.cn/gtatpvojbg.html

start) echo "启动" ;;
来源：http://hz.iojbl.cn/gtzfcxanhj.html

stop)  echo "停止" ;;
来源：http://hz.pengpengdd.cyou/gtetayrlhw.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtbcljosgt.html

esac
来源：http://hz.dianchejie.cn/gtiscsrkfn.html

[R12] for 遍历文件
来源：http://hz.ybcxt.top/gtrybxhuoh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtprowspgw.html

[R13] for 计数循环
来源：http://hz.zhengqikj.top/gtnuraiclj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.zycfv.cn/gtrsqfwaen.html

[R14] C 风格 for
来源：http://hz.316326.xyz/gthljepclx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.vqdsnc.cn/gtecnlyhcd.html

[R15] while 逐行读文件
来源：http://hz.xziqi.cn/gtxehdvabh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.daria6918.cn/gtnaqqtzxs.html

[R16] until 等待条件
来源：http://hz.c1oappe.top/gtbkqomvsa.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.shzxlz.cn/gtivlhkwbv.html

[R17] 数组定义与取值
来源：http://hz.daxiang520.top/gtgjfubdut.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtsdnyblit.html

[R18] 遍历数组
来源：http://hz.xingfuxueyuan.xyz/gtrfemewbp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.cdnleiting.top/gtfovpuqwz.html

[R19] 数组长度
来源：http://hz.zhongyouzk.top/gtyqfhsyml.html

echo "${#arr[@]}"
来源：http://hz.ywan-chungtsiang.top/gtdyyfaqzi.html

[R20] 关联数组（字典）
来源：http://hz.ppjwa.cn/gtvikwginy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtrlfdgvjq.html

[R21] 字符串长度
来源：http://hz.pengpengdd.cyou/gtqjrdigtz.html

echo "${#s}"
来源：http://hz.zhengqikj.top/gtesuosqlu.html

[R22] 截取子串
来源：http://hz.hnxiangtu.top/gtyjrpvwzw.html

echo "${s:0:5}"
来源：http://hz.shzxlz.cn/gtpnsjgadc.html

[R23] 字符串替换
来源：http://hz.ydjk.org.cn/gtaqgvizel.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.aizwys.cn/gtanbeqoqm.html

[R24] 大小写转换
来源：http://hz.zhixingplan.top/gtflfmkvij.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhaomingkeji.xyz/gtggnhexqp.html

[R25] 去后缀 / 去前缀
来源：http://hz.mhx1999.top/gtckiwpbko.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.chenjidiqi.icu/gtqpdbryhc.html

[R26] 命令替换
来源：http://hz.kuanghao11.cn/gtbvicpgww.html

now=$(date +%F); echo "$now"
来源：http://hz.ehwqpu.com/gtswexxatt.html

[R27] 算术展开
来源：http://hz.yj20258888.top/gtnzltwlze.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtvrlcwspv.html

[R28] 浮点运算
来源：http://hz.jiagoushi.top/gtiyigkdoy.html

echo "scale=2; 10/3" | bc
来源：http://hz.hongshengwenyu.top/gtklmlmwxe.html

[R29] 定义函数
来源：http://hz.hfpthk.cn/gtxfrjzjhi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj20258888.top/gtzfelzjpr.html

[R30] 函数返回状态码
来源：http://hz.ydjk.org.cn/gtuaxivcku.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.zycfv.cn/gtwovpwaar.html

[R31] 局部变量
来源：http://hz.zhengqikj.top/gtohqirjyz.html

f() { local x=1; echo "$x"; }
来源：http://hz.jianghu66.top/gtimvwdefk.html

[R32] 参数个数校验
来源：http://hz.ywan-chungtsiang.top/gtkzjvqhig.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.zhijiandao.cn/gtkrwwubtk.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtdykeopjk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ivvv.top/gtxekjzysz.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gtyrkevtsc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.zhiwuduotai.top/gtxokldehg.html

[R35] 后台执行并等待
来源：http://hz.ybcxt.top/gtltqtlqwx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hfpthk.cn/gtouhywhfc.html

[R36] 并发执行多个任务
来源：http://hz.sweek.top/gtzaomapcj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sysykeji.top/gthrsjtdsm.html

[R37] 把输出赋给变量
来源：http://hz.zdqjudy.top/gtrsipuspf.html

files=$(ls -1)
来源：http://hz.shzxlz.cn/gtarpmkkjp.html

[R38] 管道串联
来源：http://hz.shanyushiyangtech.top/gtwhfbjsbj.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sweek.top/gtzdzjeewj.html

[R39] 重定向标准输出与错误
来源：http://hz.sweek.top/gthfjhmadj.html

cmd > out.log 2>&1
来源：http://hz.pengpengdd.cyou/gtbitmqocl.html

[R40] 追加写日志
来源：http://hz.shanyushiyangtech.top/gtndrvdvyz.html

echo "log" >> out.log
来源：http://hz.wangdashe.top/gtxwdumjvr.html

[R41] 丢弃输出
来源：http://hz.hnqzz.top/gtvyngscai.html

cmd >/dev/null 2>&1
来源：http://hz.yuanzhike.top/gtwkbprons.html

[R42] 输入重定向
来源：http://hz.nanxuanxn.top/gtakevhfme.html

wc -l < a.txt
来源：http://hz.zycfv.cn/gttaqqftdq.html

[R43] 按名字查找文件
来源：http://hz.yj20258888.top/gtnzvuznng.html

find . -name "*.log" -type f
来源：http://hz.wangdashe.top/gtbeynmziz.html

[R44] 按修改时间查找
来源：http://hz.shzxlz.cn/gtwnfewfhk.html

find . -mtime -7 -type f
来源：http://hz.pengpengdd.cyou/gtcmfvkjkc.html

[R45] 批量删除
来源：http://hz.zhijiandao.cn/gtskbudlqm.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gthtcxiaia.html

[R46] 递归替换文件内容
来源：http://hz.c1oappe.top/gtaptvjxvm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinyuanbaomall.cn/gtcxxmwqck.html

[R47] sed 单行替换
来源：http://hz.tian-w.cn/gtvxakchfk.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yuanzhike.top/gtkfknsugr.html

[R48] awk 取指定列
来源：http://hz.jianghu66.top/gtoyvarlau.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtczkrcwcw.html

[R49] awk 带条件
来源：http://hz.meibo888.top/gtkozsilqw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.gotoacloud.top/gtcvwjtcup.html

[R50] awk 求和
来源：http://hz.jinghuilouyu.cn/gtjvlhptiu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cucudq.cn/gtwxmzybdk.html

[R51] 排序去重取前几
来源：http://hz.smart0.xyz/gtfardezuc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.smart0.xyz/gtslhcwwjc.html

[R52] 统计行数
来源：http://hz.andypj.xyz/gtsnlnqgui.html

wc -l a.txt
来源：http://hz.chenjidiqi.icu/gtozlqrjrj.html

[R53] 查看文件头与实时尾
来源：http://hz.hnxiangtu.top/gtfksngqpb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.xziqi.cn/gtyemgoazh.html

[R54] 比较两个文件
来源：http://hz.daria6918.cn/gtnhthinrl.html

diff a.txt b.txt
来源：http://hz.yanxiufei.cn/gtimpkjoes.html

[R55] 压缩与解压
来源：http://hz.cqqwz.cn/gtzdbokokf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.hysaishi.cn/gtiqpkypeo.html

[R56] 远程拷贝
来源：http://hz.ehwqpu.com/gtjuslfvff.html

scp file user@host:/path/
来源：http://hz.mhx1999.top/gthwekljqs.html

[R57] 远程执行命令
来源：http://hz.iojbl.cn/gtiawbfukn.html

ssh user@host 'uptime'
来源：http://hz.yj202588.top/gtbowfivhn.html

[R58] 下载文件
来源：http://hz.meibo888.top/gtzgohezqk.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yuxming.cn/gtvwujhgww.html

[R59] 发 POST JSON
来源：http://hz.jqgfzy.top/gtdnqxjylu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.meibo888.top/gtuunzteij.html

[R60] 只看 HTTP 状态码
来源：http://hz.hfpthk.cn/gtmeygvmpl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtyhgyigsg.html

[R61] 磁盘占用
来源：http://hz.haohaochexian.top/gtxnqhoxew.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtjiwwehmk.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gthwzwmorx.html

du -ah . | sort -rh | head -10
来源：http://hz.yanxiufei.cn/gtltugmodm.html

[R63] 内存与进程
来源：http://hz.andypj.xyz/gteubzqwmy.html

free -h;  ps aux | grep nginx
来源：http://hz.hnxiangtu.top/gtfjxqpoxf.html

[R64] 结束进程
来源：http://hz.hnqzz.top/gthkpqjuwm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtuvkgfrzr.html

[R65] 查看端口占用
来源：http://hz.quarkkingdee.top/gtvjodcdou.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gtupgjzfcw.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gtrxcrpfwz.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gtibhehnhv.html

[R67] 生成随机十六进制串
来源：http://hz.ivvv.top/gtauoiycrz.html

openssl rand -hex 16
来源：http://hz.yuanzhike.top/gtcueewqgm.html

[R68] 计算文件校验值
来源：http://hz.ydjk.org.cn/gtgcrpxkpx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.feifeiyinyue.top/gtlavlytgy.html

[R69] 生成随机密码
来源：http://hz.jlsjyb.cn/gtuyywving.html

head -c 16 /dev/urandom | base64
来源：http://hz.ydjk.org.cn/gtxcqwnaux.html

[R70] 时间戳与互转
来源：http://hz.hywenlv.cn/gtlsirqotx.html

date +%s;  date -d @1700000000
来源：http://hz.ehwqpu.com/gtdsfvcocg.html

[R71] 日期格式化
来源：http://hz.yueranfly.top/gtkenxhmcq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jlsjyb.cn/gtxhmyqnse.html

[R72] 等待端口就绪
来源：http://hz.yj202588.top/gtbjbgtwky.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.guowangkeji.top/gtdqdidxpp.html

[R73] 分割大日志
来源：http://hz.hfpthk.cn/gtwovginew.html

split -l 1000 big.log part_
来源：http://hz.c1oappe.top/gttmeqjrsx.html

[R74] 批量重命名
来源：http://hz.hnxiangtu.top/gtnduojgji.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.xuanzx.com/gthuzfxxvu.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtkdkwvrmi.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yanxiufei.cn/gtbacvtsoq.html

[R76] 使用临时文件
来源：http://hz.tianlin.xyz/gtkydkifco.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtnzlwytnk.html

[R77] 读取用户输入
来源：http://hz.0kj1m.cn/gtrbpreohk.html

read -rp "请输入: " ans
来源：http://hz.guannengcc.top/gtygcselry.html

[R78] 交互式菜单
来源：http://hz.yonumen.top/gtpiqmvimp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.feifeiyinyue.top/gtukioutiv.html

[R79] 解析命令行选项
来源：http://hz.ydzc1.top/gtacwyndbn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgfzy.top/gtolgdvdbs.html

[R80] 查看脚本执行耗时
来源：http://hz.hammf.cn/gtvqltawbm.html

time ./run.sh
来源：http://hz.snrcjt.cn/gthvmaothx.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gttfcrgqyg.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtslihqyte.html

================================================================================
来源：http://hz.smart0.xyz/gtzoqieisa.html

[S01] C：Hello World
来源：http://hz.cucudq.cn/gtfecflmzv.html

#include <stdio.h>
来源：http://hz.zhixingplan.top/gtyxmltcph.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cqqwz.cn/gtzvqwtfoj.html

[S02] C：变量与格式化输出
来源：http://hz.ywan-chungtsiang.top/gtxjmwsmsf.html

int a = 10; printf("%d\n", a);
来源：http://hz.vqdsnc.cn/gtqfqxuhpw.html

[S03] C：读入整数
来源：http://hz.hnxiangtu.top/gtvbhuosro.html

int x; scanf("%d", &x);
来源：http://hz.dashuyun.cn/gtqrgewvgz.html

[S04] C：字符串复制
来源：http://hz.jqgfzy.top/gtchswoino.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yuanzhike.top/gthbvzmzhm.html

[S05] C：字符串长度
来源：http://hz.dashuyun.cn/gtfpblvipv.html

strlen(s)
来源：http://hz.yj202588.top/gthbrdzoar.html

[S06] C：字符串比较
来源：http://hz.jinghuilouyu.cn/gtehkijqtb.html

strcmp(a, b) == 0
来源：http://hz.sxryk.cn/gtocgnzyte.html

[S07] C：数组遍历求和
来源：http://hz.zhiwuduotai.top/gtelhkzsdb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.mhx1999.top/gtocalubnh.html

[S08] C：动态内存分配与释放
来源：http://hz.cashguo.top/gtzrdlvtjv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.fzhhl.top/gtcrfhsous.html

[S09] C：结构体定义与初始化
来源：http://hz.cheryme.top/gtxqaubuud.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jyoumei.cn/gtfesbdbjp.html

[S10] C：指针与解引用
来源：http://hz.hnxiangtu.top/gtieymkjvd.html

int *p = &a;  *p = 5;
来源：http://hz.fzhhl.top/gtcnpwsszp.html

[S11] C：逐行读文件
来源：http://hz.wangshuangyany.cn/gtvwzdywcg.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.haohaochexian.top/gthppipsyk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.hnxiangtu.top/gtvuqgtlee.html

fclose(f);
来源：http://hz.sysykeji.top/gtzrhqtlrl.html

[S12] C：写文件
来源：http://hz.daxiang520.top/gtdzgujybb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tianlin.xyz/gtmkpcjgvf.html

[S13] C：宏定义
来源：http://hz.shanyushiyangtech.top/gtrqklrfgj.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangdashe.top/gtcqisokfc.html

[S14] C：枚举
来源：http://hz.daria6918.cn/gtbbvjzpkg.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.shzxlz.cn/gterrgvhcb.html

[S15] C：类型转换
来源：http://hz.hnqzz.top/gtxqxtobfg.html

(double) a / b
来源：http://hz.daxiang520.top/gtabafasoo.html

[S16] C：位操作置位
来源：http://hz.yj20258888.top/gtfszgpfnn.html

x |= (1 << 3);
来源：http://hz.zhixingplan.top/gtfclvpasq.html

[S17] C：安全拼接字符串
来源：http://hz.yueranfly.top/gtpbhfypqd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cqqwz.cn/gtgywrlpkd.html

[S18] C：命令行参数
来源：http://hz.cheryme.top/gtcfxwxuqi.html

int main(int argc, char **argv)
来源：http://hz.xinyue.icu/gtdotnlkjv.html

[S19] C：快速排序
来源：http://hz.zhijiandao.cn/gtkfipxfmc.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zycfv.cn/gtzqfbopaf.html

[S20] C：二分查找
来源：http://hz.fengsongda.top/gtmbprznwf.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.svipenyu.cn/gtlzsfujvb.html

[S21] C：字符类别判断
来源：http://hz.snrcjt.cn/gtbkqvvkgw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xingfuxueyuan.xyz/gtedvvhdyq.html

[S22] C：字符串转数字
来源：http://hz.sweek.top/gtxclirhzo.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhongyouzk.top/gtijopjmbn.html

[S23] C：随机数
来源：http://hz.pycfn.com/gtxsklnpml.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cheryme.top/gtwqwzqrna.html

[S24] C：获取本地时间
来源：http://hz.hnxiangtu.top/gtemugztyh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.vqdsnc.cn/gtqzncalga.html

[S25] C：内存拷贝
来源：http://hz.jqgfzy.top/gtlacbmbqh.html

memcpy(dst, src, n);
来源：http://hz.jianghu66.top/gtbjbfegst.html

[S26] C：内存清零
来源：http://hz.shuidangran.top/gtbbhramnd.html

memset(a, 0, sizeof a);
来源：http://hz.ydjk.org.cn/gtlfccsddk.html

[S27] C：定义常量
来源：http://hz.zhiwuduotai.top/gtgsfmrlih.html

const double PI = 3.14159;
来源：http://hz.zhoulong.xyz/gtwjktyhrq.html

[S28] C：静态变量
来源：http://hz.jqgfzy.top/gtkgnqlbrs.html

static int counter = 0;
来源：http://hz.xinyue.icu/gtdrvjtjvb.html

[S29] C：变参函数
来源：http://hz.hnqzz.top/gtsoxvwwlu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangtech.top/gtzvtcxvsg.html

[S30] C：头文件保护
来源：http://hz.nanxinkj.top/gtpdyujnbo.html

#ifndef X_H
来源：http://hz.cucudq.cn/gtexzivomr.html

#define X_H
来源：http://hz.ywan-chungtsiang.top/gthtlqqlfv.html

#endif
来源：http://hz.52xcode.cn/gtfclhgenl.html

[S31] C++：Hello World
来源：http://hz.ydzc1.top/gtyobfuyqj.html

#include <iostream>
来源：http://hz.zycfv.cn/gtleifxzot.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.chenjidiqi.icu/gtsegankjn.html

[S32] C++：字符串
来源：http://hz.pycfn.com/gtueuqynjw.html

std::string s = "hi";  s += "!";
来源：http://hz.316326.xyz/gtqmrmyxwf.html

[S33] C++：vector 增删
来源：http://hz.nanxinkj.top/gtnwiuokyn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.meibo888.top/gthlfqwfps.html

[S34] C++：遍历 vector
来源：http://hz.wangdashe.top/gtvzcscwfe.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.yueranfly.top/gtbnjttlnd.html

[S35] C++：map
来源：http://hz.zycfv.cn/gtjerpeuzk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xylfe.cn/gtmwgtdwtr.html

[S36] C++：unordered_map
来源：http://hz.jlsjyb.cn/gtfhgbfbnp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.gotoacloud.top/gteqpqtdgu.html

[S37] C++：set
来源：http://hz.chenlongwang.top/gtwrbtjluw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.ppjwa.cn/gtafdcamxf.html

[S38] C++：排序
来源：http://hz.smart0.xyz/gtasvacmds.html

std::sort(v.begin(), v.end());
来源：http://hz.smart0.xyz/gtlmamzshe.html

[S39] C++：自定义比较器排序
来源：http://hz.haohaochexian.top/gtimhrgcdo.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.gogol.net.cn/gtaljcldtd.html

[S40] C++：查找元素
来源：http://hz.dianchejie.cn/gtxrhttjhv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.quarkkingdee.top/gtmkcprkcy.html

[S41] C++：类与构造函数
来源：http://hz.jlsjyb.cn/gtvinnawcd.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.jyoumei.cn/gthpmmwudt.html

[S42] C++：继承与虚函数
来源：http://hz.xziqi.cn/gtvjgsxyhp.html

class B : public Base { public: void f() override {} };
来源：http://hz.yuanzhike.top/gtyhxallll.html

[S43] C++：智能指针
来源：http://hz.andypj.xyz/gtlnsfkytn.html

auto p = std::make_unique<int>(5);
来源：http://hz.xingfuxueyuan.xyz/gtvrmecrjr.html

[S44] C++：引用传参
来源：http://hz.ywan-chungtsiang.top/gtxwcvolyn.html

void inc(int &x) { ++x; }
来源：http://hz.dashuyun.cn/gtvddphnbm.html

[S45] C++：lambda
来源：http://hz.tian-w.cn/gtbffknnud.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.smart0.xyz/gtgayljwnu.html

[S46] C++：函数模板
来源：http://hz.yj202588.top/gthobiyqjy.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.jinqigfzy.top/gthrmrusrd.html

[S47] C++：结构化绑定遍历
来源：http://hz.yj20258888.top/gtjvljkzaa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.shanyushiyangkeji.top/gtinhtnody.html

[S48] C++：逐行读文件
来源：http://hz.0kj1m.cn/gtzpehevot.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.snrcjt.cn/gtthgqctsm.html


<!-- 参考信息 -->