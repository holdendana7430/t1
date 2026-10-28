代发 wailian999

[Q84] 去除首尾空格
来源：http://hz.guowangkeji.top/gtttobupza.html

SELECT TRIM(name) FROM users;
来源：http://hz.kuanghao11.cn/gttswgnnlp.html

[Q85] 数值取整
来源：http://hz.haohaochexian.top/gttzslnomd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.nwbrower.top/gthyoabxnn.html

[Q86] 读取 JSON 字段
来源：http://hz.ehwqpu.com/gtuifhsxbh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.jinghuilouyu.cn/gtvageqevz.html

[Q87] JSON 字段做条件
来源：http://hz.hongshengwenyu.top/gtehghwqrf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.haohaochexian.top/gtffcougdq.html

[Q88] 行转列（条件聚合）
来源：http://hz.iojbl.cn/gtnytlyvsf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gtwovlqddo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.wangdashe.top/gtdazkbwpt.html

[Q89] 判断表是否存在
来源：http://hz.yj20258.top/gtsgrdibdz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yvedp.cn/gthfjnfxeq.html

[Q90] 生成序号列
来源：http://hz.jianghu66.top/gtajhdrvgm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuanzx.com/gthhvjglwx.html

================================================================================
来源：http://hz.hammf.cn/gtapkzwrfk.html

R. Bash 专题
来源：http://hz.daria6918.cn/gtebghxnmz.html

================================================================================
来源：http://hz.bjfxy.top/gteejrrykj.html

[R01] shebang 与严格模式
来源：http://hz.ehwqpu.com/gtwbvrnadk.html

#!/usr/bin/env bash
来源：http://hz.shuidangran.top/gtcyvkoelm.html

set -euo pipefail
来源：http://hz.gaohongyu789.top/gtrypodvpk.html

[R02] 变量赋值与使用
来源：http://hz.jqgufenzy.top/gttiquzxit.html

name="Tom"; echo "$name"
来源：http://hz.xinyue.icu/gtsooodpub.html

[R03] 只读变量
来源：http://hz.cdnleiting.top/gtnhvjeuux.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtvxhdtnvi.html

[R04] 位置参数
来源：http://hz.feifeiyinyue.top/gtjntxzcuh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zdqjudy.top/gtyxmkipov.html

[R05] 参数默认值
来源：http://hz.pycfn.com/gthjecifdu.html

name="${1:-default}"
来源：http://hz.pycfn.com/gtwrcyarie.html

[R06] 判断命令是否存在
来源：http://hz.redwolf501.top/gtxwrgragx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hnxiangtu.top/gtgelhytnr.html

[R07] if 判断文件
来源：http://hz.bjfxy.top/gtssiwcbam.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.hnxiangtu.top/gtwabynuba.html

[R08] 数值比较
来源：http://hz.jqgufenzy.top/gtkkhayshh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tianlin.xyz/gtpagrqrji.html

[R09] 字符串比较
来源：http://hz.meibo888.top/gthjqlfbom.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.wangdashe.top/gtsafopvoy.html

[R10] 正则匹配
来源：http://hz.tanke756.top/gttdpsjibl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zycfv.cn/gtadbeuneb.html

[R11] case 多分支
来源：http://hz.sufxvd.cn/gtclmcldee.html

case "$1" in
来源：http://hz.jlsjyb.cn/gtazaopyrn.html

start) echo "启动" ;;
来源：http://hz.hfpthk.cn/gtppzzrzyv.html

stop)  echo "停止" ;;
来源：http://hz.shangyingyoupin.top/gtnltbeito.html

*)     echo "未知命令" ;;
来源：http://hz.quarkkingdee.top/gtannsbica.html

esac
来源：http://hz.gotoacloud.top/gtonmrmmhv.html

[R12] for 遍历文件
来源：http://hz.0kj1m.cn/gtkyoyajbp.html

for f in *.txt; do echo "$f"; done
来源：http://hz.chenzaomai.com/gtvtfpgxsm.html

[R13] for 计数循环
来源：http://hz.shzxlz.cn/gtazxkpjuv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.iojbl.cn/gtgpgffjdt.html

[R14] C 风格 for
来源：http://hz.dianchejie.cn/gtsjyfxwfq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hywenlv.cn/gtdxsxcmiw.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gttqbjaisw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuxming.cn/gtczkwahnh.html

[R16] until 等待条件
来源：http://hz.bjfxy.top/gtzehtphrz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtsrvagiwb.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gthsnjjlre.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yj202588.top/gttkbqcqtk.html

[R18] 遍历数组
来源：http://hz.zhengqikj.top/gttvttdrga.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj20258.top/gtnvltsgwg.html

[R19] 数组长度
来源：http://hz.shuidangran.top/gtxlpmugyz.html

echo "${#arr[@]}"
来源：http://hz.zdqjudy.top/gtvpoomhlv.html

[R20] 关联数组（字典）
来源：http://hz.gotoacloud.top/gtwckyrhrt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gthigjwvrs.html

[R21] 字符串长度
来源：http://hz.nwbrower.top/gtxdmjkxyq.html

echo "${#s}"
来源：http://hz.fzhhl.top/gtkvilamcy.html

[R22] 截取子串
来源：http://hz.xuetiantiany.cn/gtxzelirqq.html

echo "${s:0:5}"
来源：http://hz.52xcode.cn/gthuviltal.html

[R23] 字符串替换
来源：http://hz.gotoacloud.top/gtnsakspjz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zhijiandao.cn/gtgucyhszm.html

[R24] 大小写转换
来源：http://hz.hongshengwenyu.top/gtlogekvxc.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.svipenyu.cn/gtlbybjtes.html

[R25] 去后缀 / 去前缀
来源：http://hz.zycfv.cn/gtpggaburt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.smart0.xyz/gtkobndzev.html

[R26] 命令替换
来源：http://hz.quarkkingdee.top/gtayngkbpe.html

now=$(date +%F); echo "$now"
来源：http://hz.guowangkeji.top/gtxwisxhfp.html

[R27] 算术展开
来源：http://hz.hongshengwenyu.top/gtusjdbqhs.html

echo $((1 + 2 * 3))
来源：http://hz.xziqi.cn/gtprnekecj.html

[R28] 浮点运算
来源：http://hz.meibo888.top/gtanwvvcan.html

echo "scale=2; 10/3" | bc
来源：http://hz.tanke756.top/gtbljuumsg.html

[R29] 定义函数
来源：http://hz.zhoulong.xyz/gtwmlfvbjz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinqigufen.top/gtsmmurqyk.html

[R30] 函数返回状态码
来源：http://hz.nanxinkj.top/gtmtyadfpc.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yonumen.top/gtnxjecyrs.html

[R31] 局部变量
来源：http://hz.9152youxi.cn/gtkvkhbvzc.html

f() { local x=1; echo "$x"; }
来源：http://hz.fzhhl.top/gtpekkcpxv.html

[R32] 参数个数校验
来源：http://hz.zhaomingkeji.xyz/gtraaxiaxm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hywenlv.cn/gtplawsiqv.html

[R33] 捕获错误并提示行号
来源：http://hz.kuanghao11.cn/gtyseeooah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.tianlin.xyz/gtivsjyzdq.html

[R34] 退出时清理
来源：http://hz.aibaodan.cn/gtelxkhrcr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.cdnleiting.top/gtumdvlwqj.html

[R35] 后台执行并等待
来源：http://hz.havefunace.top/gtixaiwxue.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.birdmap.top/gtutliehqs.html

[R36] 并发执行多个任务
来源：http://hz.ehwqpu.com/gtusnqcayb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.pycfn.com/gtagnkwswd.html

[R37] 把输出赋给变量
来源：http://hz.jinghuilouyu.cn/gtdzwrgxsz.html

files=$(ls -1)
来源：http://hz.guannengcc.top/gtwmnhpzat.html

[R38] 管道串联
来源：http://hz.sufxvd.cn/gthwtxxrmh.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daxiang520.top/gtgifiyatl.html

[R39] 重定向标准输出与错误
来源：http://hz.zhongyouzk.top/gtpbdrxckf.html

cmd > out.log 2>&1
来源：http://hz.shanyushiyangkeji.top/gtetsfnjgv.html

[R40] 追加写日志
来源：http://hz.redwolf501.top/gtbnuaxgmb.html

echo "log" >> out.log
来源：http://hz.ehwqpu.com/gteoknxkbq.html

[R41] 丢弃输出
来源：http://hz.cucudq.cn/gtjlmvaohm.html

cmd >/dev/null 2>&1
来源：http://hz.chenzaomai.com/gtuttcndsf.html

[R42] 输入重定向
来源：http://hz.xinyue.icu/gtyxepmbxr.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gtfvedvhtm.html

[R43] 按名字查找文件
来源：http://hz.shanyushiyangtech.top/gtsisfhllr.html

find . -name "*.log" -type f
来源：http://hz.aizwys.cn/gtvikiztrh.html

[R44] 按修改时间查找
来源：http://hz.pengpengdd.cyou/gtbfonlotq.html

find . -mtime -7 -type f
来源：http://hz.shanyushiyangkeji.top/gtvlyknsuv.html

[R45] 批量删除
来源：http://hz.feifeiyinyue.top/gtqrqjklnx.html

find . -name "*.tmp" -delete
来源：http://hz.wangshuangyany.cn/gtketwqctp.html

[R46] 递归替换文件内容
来源：http://hz.wangshuangyany.cn/gtmytscknw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cdnleiting.top/gtpikwapof.html

[R47] sed 单行替换
来源：http://hz.shanyushiyangkeji.top/gtqjuyrojy.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.birdmap.top/gtwaibwxgm.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gthpexbyqi.html

awk '{print $1, $3}' a.txt
来源：http://hz.316326.xyz/gtwokxknmz.html

[R49] awk 带条件
来源：http://hz.shanyushiyangkeji.top/gtvhhcfqbh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.tian-w.cn/gtbyppbbib.html

[R50] awk 求和
来源：http://hz.havefunace.top/gteifqnhbl.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.zhijiandao.cn/gtwcdckciv.html

[R51] 排序去重取前几
来源：http://hz.redwolf501.top/gtvuckfmqt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenjidiqi.icu/gtonbobxce.html

[R52] 统计行数
来源：http://hz.xziqi.cn/gtzvigrvxy.html

wc -l a.txt
来源：http://hz.jyoumei.cn/gtjovmdbni.html

[R53] 查看文件头与实时尾
来源：http://hz.zhixingplan.top/gtpfxqfikp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jyoumei.cn/gtqxeifnil.html

[R54] 比较两个文件
来源：http://hz.shanyushiyangtech.top/gtdawweriu.html

diff a.txt b.txt
来源：http://hz.chenzaomai.com/gtdtwkhpfl.html

[R55] 压缩与解压
来源：http://hz.zhijiandao.cn/gtjgsfljte.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gtwisabolm.html

[R56] 远程拷贝
来源：http://hz.cdnleiting.top/gtfjrikjde.html

scp file user@host:/path/
来源：http://hz.0kj1m.cn/gtnwxdhvdr.html

[R57] 远程执行命令
来源：http://hz.0kj1m.cn/gtgjegueaj.html

ssh user@host 'uptime'
来源：http://hz.pengpengdd.cyou/gtiondxhaz.html

[R58] 下载文件
来源：http://hz.0kj1m.cn/gtlomjgjqg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jinqigfzy.top/gtweyfluyp.html

[R59] 发 POST JSON
来源：http://hz.zdqjudy.top/gtgnbdoscf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.cdnleiting.top/gtsigylqck.html

[R60] 只看 HTTP 状态码
来源：http://hz.dashuyun.cn/gtojtlarfw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.316326.xyz/gtdsynywrf.html

[R61] 磁盘占用
来源：http://hz.pycfn.com/gtlbvfrybl.html

df -h;  du -sh *
来源：http://hz.nwbrower.top/gtfnhkerdb.html

[R62] 找最占空间的文件
来源：http://hz.xziqi.cn/gtwvzxcdcg.html

du -ah . | sort -rh | head -10
来源：http://hz.sxryk.cn/gtcdnqxtkk.html

[R63] 内存与进程
来源：http://hz.nanxinkj.top/gtzvlajbug.html

free -h;  ps aux | grep nginx
来源：http://hz.guannengcc.top/gtongnselc.html

[R64] 结束进程
来源：http://hz.smart0.xyz/gtjhjaplgp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sweek.top/gtqclpypkp.html

[R65] 查看端口占用
来源：http://hz.zhiwuduotai.top/gtexxeyexu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenlongwang.top/gtrzrolyoa.html

[R66] 定时任务
来源：http://hz.zhiwuduotai.top/gtnqpidlvw.html

crontab -e;  crontab -l
来源：http://hz.c1oappe.top/gtlteetolh.html

[R67] 生成随机十六进制串
来源：http://hz.ybcxt.top/gtdrocjggt.html

openssl rand -hex 16
来源：http://hz.yj20258.top/gttxohzbnr.html

[R68] 计算文件校验值
来源：http://hz.redwolf501.top/gtynvkfslf.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.fengsongda.top/gthhbizcbc.html

[R69] 生成随机密码
来源：http://hz.yangfankeji.com/gtyapvcaon.html

head -c 16 /dev/urandom | base64
来源：http://hz.jinqigfzy.top/gtanldbetw.html

[R70] 时间戳与互转
来源：http://hz.aibaodan.cn/gtvtqsxwep.html

date +%s;  date -d @1700000000
来源：http://hz.yangfankeji.com/gtjhbhslmc.html

[R71] 日期格式化
来源：http://hz.jlsjyb.cn/gtqstkydrt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.9152youxi.cn/gtulmrcyod.html

[R72] 等待端口就绪
来源：http://hz.hnqzz.top/gtnfrjrtnm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.meibo888.top/gtwevulhle.html

[R73] 分割大日志
来源：http://hz.shuidangran.top/gtcmexzrsf.html

split -l 1000 big.log part_
来源：http://hz.xziqi.cn/gtmtwbbpga.html

[R74] 批量重命名
来源：http://hz.quarkkingdee.top/gtyghwlwra.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhijiandao.cn/gtjfiaysch.html

[R75] 导出环境变量
来源：http://hz.andypj.xyz/gtyfmzeblb.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.tanke756.top/gtdqyhjdkn.html

[R76] 使用临时文件
来源：http://hz.jqgfzy.top/gtuiqcyuwt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yueranfly.top/gtokunoith.html

[R77] 读取用户输入
来源：http://hz.chenzaomai.com/gtqutjpfgn.html

read -rp "请输入: " ans
来源：http://hz.0kj1m.cn/gtwmqwrexu.html

[R78] 交互式菜单
来源：http://hz.bjfxy.top/gtukpcfkpr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tian-w.cn/gtvwclgutz.html

[R79] 解析命令行选项
来源：http://hz.shanyushiyangkeji.top/gtzjltfrtf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.daxiang520.top/gthudplvgz.html

[R80] 查看脚本执行耗时
来源：http://hz.guowangkeji.top/gttgsawvzb.html

time ./run.sh
来源：http://hz.shangyingyoupin.top/gtpxonndqr.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtqczehxka.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtmujpstia.html

================================================================================
来源：http://hz.yuxming.cn/gtkufxrmdr.html

[S01] C：Hello World
来源：http://hz.gaohongyu789.top/gtrvbqpkhu.html

#include <stdio.h>
来源：http://hz.shzxlz.cn/gtguloomeo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xinyue.icu/gtekbupoay.html

[S02] C：变量与格式化输出
来源：http://hz.nwbrower.top/gtddgcqwmu.html

int a = 10; printf("%d\n", a);
来源：http://hz.hnqzz.top/gtumncmsjb.html

[S03] C：读入整数
来源：http://hz.zhongyouzk.top/gtdjnbegpp.html

int x; scanf("%d", &x);
来源：http://hz.xingfuxueyuan.xyz/gttozltyiy.html

[S04] C：字符串复制
来源：http://hz.gzhubu.top/gticxltgnz.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.bjfxy.top/gtlrmfhiap.html

[S05] C：字符串长度
来源：http://hz.gogol.net.cn/gtdglrdshd.html

strlen(s)
来源：http://hz.shanyushiyangtech.top/gtiatmlavg.html

[S06] C：字符串比较
来源：http://hz.c1oappe.top/gtnfmgnbgf.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtkhpgnzxi.html

[S07] C：数组遍历求和
来源：http://hz.sufxvd.cn/gtyapmnadw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yj20258888.top/gtthtfprdb.html

[S08] C：动态内存分配与释放
来源：http://hz.daxiang520.top/gtehvhktyw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.sufxvd.cn/gtksnhinyy.html

[S09] C：结构体定义与初始化
来源：http://hz.gzhubu.top/gtvzubtqzh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.jianghu66.top/gtmodafiky.html

[S10] C：指针与解引用
来源：http://hz.svipenyu.cn/gtdeiupfqn.html

int *p = &a;  *p = 5;
来源：http://hz.kuanghao11.cn/gtfvrzykdx.html

[S11] C：逐行读文件
来源：http://hz.9152youxi.cn/gtxlldeise.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.ywan-chungtsiang.top/gtjeyevzdv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.andypj.xyz/gtegnqcxqi.html

fclose(f);
来源：http://hz.zhongyouzk.top/gtdgtwutgv.html

[S12] C：写文件
来源：http://hz.zhixingplan.top/gtgksrnnaz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yueranfly.top/gtflaoiplm.html

[S13] C：宏定义
来源：http://hz.chenjidiqi.icu/gtnwwwcwrn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.zhixingplan.top/gtmdeydcbk.html

[S14] C：枚举
来源：http://hz.pengpengdd.cyou/gtrhobusmk.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.tanke756.top/gtbkarsucr.html

[S15] C：类型转换
来源：http://hz.c1oappe.top/gtfylvqtqk.html

(double) a / b
来源：http://hz.bjfxy.top/gtfgvkykba.html

[S16] C：位操作置位
来源：http://hz.shanyushiyangkeji.top/gtppxykuvl.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtgomvmbea.html

[S17] C：安全拼接字符串
来源：http://hz.shangyingyoupin.top/gtvtljxfyg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.cashguo.top/gtgbivcbxn.html

[S18] C：命令行参数
来源：http://hz.jinqigfzy.top/gtwvpqiezd.html

int main(int argc, char **argv)
来源：http://hz.shangyingyoupin.top/gtwbnfcllc.html

[S19] C：快速排序
来源：http://hz.mhx1999.top/gtwqcvgwyu.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.316326.xyz/gtkpfzmygl.html

[S20] C：二分查找
来源：http://hz.hongshengwenyu.top/gtvywxqhch.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtnapvjqnk.html

[S21] C：字符类别判断
来源：http://hz.haohaochexian.top/gtwdkekdwe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.ehwqpu.com/gtiaeawllv.html

[S22] C：字符串转数字
来源：http://hz.zdqjudy.top/gtoqjuzmpe.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.yuxming.cn/gtofhfyqhg.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtapqlvzoy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.kuanghao11.cn/gtdjxphygc.html

[S24] C：获取本地时间
来源：http://hz.yonumen.top/gtpbnsthhf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.bjfxy.top/gteovmdkre.html

[S25] C：内存拷贝
来源：http://hz.jinyuanbaomall.cn/gtumosxdnq.html

memcpy(dst, src, n);
来源：http://hz.ehwqpu.com/gtvlzvcdvw.html

[S26] C：内存清零
来源：http://hz.jinqigfzy.top/gtblyxixhp.html

memset(a, 0, sizeof a);
来源：http://hz.dashuyun.cn/gtseujrgtt.html

[S27] C：定义常量
来源：http://hz.jyoumei.cn/gtfkllpdez.html

const double PI = 3.14159;
来源：http://hz.redwolf501.top/gtmkhavsfk.html

[S28] C：静态变量
来源：http://hz.yangfankeji.com/gtisglject.html

static int counter = 0;
来源：http://hz.jinyuanbaomall.cn/gtpmmcwzco.html

[S29] C：变参函数
来源：http://hz.haohaochexian.top/gtstlmfwaj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.jianghu66.top/gtxxfwlzzp.html

[S30] C：头文件保护
来源：http://hz.yanxiufei.cn/gttmuypaiv.html

#ifndef X_H
来源：http://hz.aizwys.cn/gtjjhjdjhl.html

#define X_H
来源：http://hz.c1oappe.top/gtllzpnlue.html

#endif
来源：http://hz.xylfe.cn/gtmfiyrvqv.html

[S31] C++：Hello World
来源：http://hz.daria6918.cn/gthmtenefx.html

#include <iostream>
来源：http://hz.tanke756.top/gtnjwgviwx.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.tanke756.top/gtftgrnkuq.html

[S32] C++：字符串
来源：http://hz.gogol.net.cn/gtahtytxvl.html

std::string s = "hi";  s += "!";
来源：http://hz.yuxming.cn/gtszpsbbtt.html

[S33] C++：vector 增删
来源：http://hz.dashuyun.cn/gtnbuylhtg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.pycfn.com/gtkaobciqq.html

[S34] C++：遍历 vector
来源：http://hz.redwolf501.top/gtifqzewqn.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.xinyue.icu/gtjtzrwtfx.html

[S35] C++：map
来源：http://hz.ehwqpu.com/gtrboxktbk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtgyojsdti.html

[S36] C++：unordered_map
来源：http://hz.haohaochexian.top/gtvntocqmp.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.quarkkingdee.top/gtnrmejzlm.html

[S37] C++：set
来源：http://hz.yanxiufei.cn/gtchhbzsre.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sxryk.cn/gtlawnfilw.html

[S38] C++：排序
来源：http://hz.cashguo.top/gtxgwfxtrd.html

std::sort(v.begin(), v.end());
来源：http://hz.jqgfzy.top/gtnhvgzppu.html

[S39] C++：自定义比较器排序
来源：http://hz.fengsongda.top/gtxpclfglz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.cashguo.top/gtzjtohbrf.html

[S40] C++：查找元素
来源：http://hz.sxryk.cn/gtdstqlewt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.feifeiyinyue.top/gtykqezcyj.html

[S41] C++：类与构造函数
来源：http://hz.chenlongwang.top/gtppdbkeis.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.ybcxt.top/gtngpcexig.html

[S42] C++：继承与虚函数
来源：http://hz.zhoulong.xyz/gteppmgihi.html

class B : public Base { public: void f() override {} };
来源：http://hz.birdmap.top/gtbguarrce.html

[S43] C++：智能指针
来源：http://hz.cdnleiting.top/gtiaawgcig.html

auto p = std::make_unique<int>(5);
来源：http://hz.cucudq.cn/gtipkmknwn.html

[S44] C++：引用传参
来源：http://hz.xuanzx.com/gtdqahhfex.html

void inc(int &x) { ++x; }
来源：http://hz.jinghuilouyu.cn/gtaaodmtpy.html

[S45] C++：lambda
来源：http://hz.hysaishi.cn/gtpwgouayg.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.xinyue.icu/gtyqqlxann.html

[S46] C++：函数模板
来源：http://hz.yongpay.top/gttetnbfin.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.sysykeji.top/gtukqndezq.html

[S47] C++：结构化绑定遍历
来源：http://hz.ivvv.top/gtocbhfyih.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.hywenlv.cn/gtljzxyvcp.html

[S48] C++：逐行读文件
来源：http://hz.9152youxi.cn/gtihpwsjto.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gaohongyu789.top/gtmscjzlgz.html

while (std::getline(in, line)) { }
来源：http://hz.svipenyu.cn/gtmwtjnnzj.html

[S49] C++：写文件
来源：http://hz.zhijiandao.cn/gtqrvzbxgg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.xziqi.cn/gtrcqkcbpe.html

[S50] C++：格式化数字
来源：http://hz.guowangkeji.top/gtfuectnsf.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.xylfe.cn/gtayxbwrjt.html

[S51] C++：显式类型转换
来源：http://hz.xuanzx.com/gtimwtsmyk.html

static_cast<double>(a) / b
来源：http://hz.feifeiyinyue.top/gthopmbqbo.html

[S52] C++：const 与 noexcept
来源：http://hz.gzhubu.top/gtkhyqmfoe.html

int size() const noexcept { return n_; }
来源：http://hz.sxryk.cn/gtqrjcxyxj.html

[S53] C++：移动语义
来源：http://hz.gotoacloud.top/gtdfaczsiw.html

std::vector<int> w = std::move(v);
来源：http://hz.yj202588.top/gtkkoluvzn.html

[S54] C++：异常处理
来源：http://hz.vqdsnc.cn/gtfipcguui.html


<!-- 参考信息 -->