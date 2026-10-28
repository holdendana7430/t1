代发 wailian999

[Q80] 字符串截取
来源：http://hz.cqqwz.cn/gtahucxxwk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shanyushiyangtech.top/gtschobony.html

[Q81] 字符串替换
来源：http://hz.0kj1m.cn/gtybuwnzjb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.c1oappe.top/gtmexievdo.html

[Q82] 字符长度与字节长度
来源：http://hz.ppjwa.cn/gtfwzyyjvx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.ydjk.org.cn/gtidcmzfid.html

[Q83] 大小写转换
来源：http://hz.ydzc1.top/gtcjobcfyz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.nanxuanxn.top/gtkvhsqpyx.html

[Q84] 去除首尾空格
来源：http://hz.nanxinkj.top/gttbnefoev.html

SELECT TRIM(name) FROM users;
来源：http://hz.guannengcc.top/gtxwsvrcrn.html

[Q85] 数值取整
来源：http://hz.zhixingplan.top/gtrilkmgmi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.pengpengdd.cyou/gtmmrbtnrz.html

[Q86] 读取 JSON 字段
来源：http://hz.hnxiangtu.top/gtfaydyjvw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nwbrower.top/gtkglrybmj.html

[Q87] JSON 字段做条件
来源：http://hz.xuanzx.com/gtfyshvopc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yuanzhike.top/gtloizgkzh.html

[Q88] 行转列（条件聚合）
来源：http://hz.feifeiyinyue.top/gtlarcvqiv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.52xcode.cn/gtyyrnoyiv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.xylfe.cn/gtaztwguyn.html

[Q89] 判断表是否存在
来源：http://hz.xuetiantiany.cn/gtlvyjgppz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.guowangkeji.top/gtrhpehnvt.html

[Q90] 生成序号列
来源：http://hz.dashuyun.cn/gtggeeznuq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.316326.xyz/gtintdtzeo.html

================================================================================
来源：http://hz.jianghu66.top/gtakihzgfm.html

R. Bash 专题
来源：http://hz.haohaochexian.top/gttreniiqh.html

================================================================================
来源：http://hz.mhx1999.top/gtczkwjiko.html

[R01] shebang 与严格模式
来源：http://hz.andypj.xyz/gtwvavlrkp.html

#!/usr/bin/env bash
来源：http://hz.nanxinkj.top/gtuarvsmrz.html

set -euo pipefail
来源：http://hz.zhijiandao.cn/gtwzleboap.html

[R02] 变量赋值与使用
来源：http://hz.cheryme.top/gtxwgizlnj.html

name="Tom"; echo "$name"
来源：http://hz.jinqigfzy.top/gtzhcselno.html

[R03] 只读变量
来源：http://hz.jyoumei.cn/gtlcwrcgxy.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtdmwhizer.html

[R04] 位置参数
来源：http://hz.havefunace.top/gttjysqmcb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xuetiantiany.cn/gtywbfnygm.html

[R05] 参数默认值
来源：http://hz.cucudq.cn/gtinwfyrql.html

name="${1:-default}"
来源：http://hz.fzhhl.top/gtofbxakpn.html

[R06] 判断命令是否存在
来源：http://hz.gaohongyu789.top/gtxnjvpeen.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jyoumei.cn/gttdpjlqdv.html

[R07] if 判断文件
来源：http://hz.xylfe.cn/gtjwzvjbsl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtvpxmzsex.html

[R08] 数值比较
来源：http://hz.ydjk.org.cn/gtlwxxgsjj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.tanke756.top/gtmeqnphcm.html

[R09] 字符串比较
来源：http://hz.hywenlv.cn/gtfbuswwmb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.bjfxy.top/gtfdtedgia.html

[R10] 正则匹配
来源：http://hz.zdqjudy.top/gtlalmytom.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hongshengwenyu.top/gtmlsxcgll.html

[R11] case 多分支
来源：http://hz.xingfuxueyuan.xyz/gtmwllrwbp.html

case "$1" in
来源：http://hz.quarkkingdee.top/gtzdjgjdgf.html

start) echo "启动" ;;
来源：http://hz.jinyuanbaomall.cn/gtedkrnyxs.html

stop)  echo "停止" ;;
来源：http://hz.snrcjt.cn/gtmmjfqqnc.html

*)     echo "未知命令" ;;
来源：http://hz.tian-w.cn/gtdeslzgov.html

esac
来源：http://hz.cdnleiting.top/gtsrajvuez.html

[R12] for 遍历文件
来源：http://hz.pengpengdd.cyou/gtxdsfsziu.html

for f in *.txt; do echo "$f"; done
来源：http://hz.hfpthk.cn/gtuodtwerz.html

[R13] for 计数循环
来源：http://hz.jiagoushi.top/gtmdcxsmod.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.redwolf501.top/gtgediownq.html

[R14] C 风格 for
来源：http://hz.ppjwa.cn/gtprccxhzs.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.ybcxt.top/gtryurugbq.html

[R15] while 逐行读文件
来源：http://hz.cucudq.cn/gtvhpozhan.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.aibaodan.cn/gtduosssrf.html

[R16] until 等待条件
来源：http://hz.c1oappe.top/gtifiykebg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.gaohongyu789.top/gtuojhpjkg.html

[R17] 数组定义与取值
来源：http://hz.cqqwz.cn/gttoajztyu.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yongpay.top/gtiuxymevq.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gthumfmubu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.gaohongyu789.top/gtzzuoufjx.html

[R19] 数组长度
来源：http://hz.yonumen.top/gtogaszasn.html

echo "${#arr[@]}"
来源：http://hz.xinyue.icu/gtidgotxbs.html

[R20] 关联数组（字典）
来源：http://hz.zhaomingkeji.xyz/gtzfvbctfk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fzhhl.top/gtpdnnlpsg.html

[R21] 字符串长度
来源：http://hz.xingfuxueyuan.xyz/gtqntnjmab.html

echo "${#s}"
来源：http://hz.yuxming.cn/gtebbyqydp.html

[R22] 截取子串
来源：http://hz.xziqi.cn/gtedgfkack.html

echo "${s:0:5}"
来源：http://hz.chenlongwang.top/gttybswzvu.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtlsdoagea.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.tianlin.xyz/gtodnseunp.html

[R24] 大小写转换
来源：http://hz.chenjidiqi.icu/gtrdwkqjrw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.hnqzz.top/gtvatyfozf.html

[R25] 去后缀 / 去前缀
来源：http://hz.tian-w.cn/gtbmezmmjb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.iojbl.cn/gtnfirvren.html

[R26] 命令替换
来源：http://hz.redwolf501.top/gtbliuxbgp.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtasofgktg.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtijprdvbz.html

echo $((1 + 2 * 3))
来源：http://hz.xuanzx.com/gtsejxmdek.html

[R28] 浮点运算
来源：http://hz.daria6918.cn/gtsoycqnwm.html

echo "scale=2; 10/3" | bc
来源：http://hz.pycfn.com/gtaxhjiuss.html

[R29] 定义函数
来源：http://hz.sufxvd.cn/gtcxkpylig.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.feifeiyinyue.top/gtkxsrbxns.html

[R30] 函数返回状态码
来源：http://hz.jyoumei.cn/gtijnxwpxf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.bjfxy.top/gtefxspuee.html

[R31] 局部变量
来源：http://hz.hammf.cn/gtdgitzert.html

f() { local x=1; echo "$x"; }
来源：http://hz.gogol.net.cn/gtiivjwgcc.html

[R32] 参数个数校验
来源：http://hz.yj20258.top/gttdueomoe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.hongshengwenyu.top/gtgjpbopdi.html

[R33] 捕获错误并提示行号
来源：http://hz.yonumen.top/gtipvotvwa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.jinqigufen.top/gtprfdzzlf.html

[R34] 退出时清理
来源：http://hz.shuidangran.top/gtnftvtcea.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.snrcjt.cn/gttggxcawl.html

[R35] 后台执行并等待
来源：http://hz.hywenlv.cn/gtfkxalwqb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.gogol.net.cn/gthpvixegc.html

[R36] 并发执行多个任务
来源：http://hz.yonumen.top/gtahjiqnyx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtlhmmdybq.html

[R37] 把输出赋给变量
来源：http://hz.chenjidiqi.icu/gtlglrdcoq.html

files=$(ls -1)
来源：http://hz.gogol.net.cn/gtnwrkvhtj.html

[R38] 管道串联
来源：http://hz.jiagoushi.top/gtfuzfctfs.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhijiandao.cn/gtouwaagza.html

[R39] 重定向标准输出与错误
来源：http://hz.yongpay.top/gttunaeffi.html

cmd > out.log 2>&1
来源：http://hz.sufxvd.cn/gtpzqydkeu.html

[R40] 追加写日志
来源：http://hz.guowangkeji.top/gtdkwglcbp.html

echo "log" >> out.log
来源：http://hz.quarkkingdee.top/gtulisxwth.html

[R41] 丢弃输出
来源：http://hz.guannengcc.top/gtuyvzjlls.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gtakiurfzy.html

[R42] 输入重定向
来源：http://hz.fengsongda.top/gtzvuwgnna.html

wc -l < a.txt
来源：http://hz.chenzaomai.com/gtkvuinqpv.html

[R43] 按名字查找文件
来源：http://hz.ydzc1.top/gtylnsjniv.html

find . -name "*.log" -type f
来源：http://hz.zhiwuduotai.top/gtbmslcneh.html

[R44] 按修改时间查找
来源：http://hz.shanyushiyangkeji.top/gtsdxlaubh.html

find . -mtime -7 -type f
来源：http://hz.jianghu66.top/gtnqkqomvp.html

[R45] 批量删除
来源：http://hz.iojbl.cn/gtguhqmoan.html

find . -name "*.tmp" -delete
来源：http://hz.daria6918.cn/gtmuedwloj.html

[R46] 递归替换文件内容
来源：http://hz.316326.xyz/gtncqrcole.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinghuilouyu.cn/gtjekosvwd.html

[R47] sed 单行替换
来源：http://hz.nanxinkj.top/gtbpshzuir.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.redwolf501.top/gtomgznaem.html

[R48] awk 取指定列
来源：http://hz.zhengqikj.top/gtkyfkhbsj.html

awk '{print $1, $3}' a.txt
来源：http://hz.gaohongyu789.top/gtdrbyjvco.html

[R49] awk 带条件
来源：http://hz.yueranfly.top/gtcyrjtcxr.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.birdmap.top/gtwavesnfo.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtjskaoqqu.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.ivvv.top/gtibkabqbx.html

[R51] 排序去重取前几
来源：http://hz.hywenlv.cn/gtcvfluqbs.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cucudq.cn/gtezccxnhh.html

[R52] 统计行数
来源：http://hz.gogol.net.cn/gtpphrnmte.html

wc -l a.txt
来源：http://hz.xinyue.icu/gthhnbygae.html

[R53] 查看文件头与实时尾
来源：http://hz.zycfv.cn/gtyyyqvhrz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.wangshuangyany.cn/gtsulwzenz.html

[R54] 比较两个文件
来源：http://hz.jlsjyb.cn/gtzxdiqwhs.html

diff a.txt b.txt
来源：http://hz.chenlongwang.top/gtlppicdik.html

[R55] 压缩与解压
来源：http://hz.yvedp.cn/gtnlfrochu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jiagoushi.top/gtfiikkbnm.html

[R56] 远程拷贝
来源：http://hz.ydzc1.top/gtckqwndig.html

scp file user@host:/path/
来源：http://hz.yj20258.top/gtcoyoakqg.html

[R57] 远程执行命令
来源：http://hz.jinyuanbaomall.cn/gtkpiguuhu.html

ssh user@host 'uptime'
来源：http://hz.xinyue.icu/gtmkixjtks.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtwgwsbxhq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.zhoulong.xyz/gtwmqivbgk.html

[R59] 发 POST JSON
来源：http://hz.shuidangran.top/gtwufkxzha.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ydjk.org.cn/gtqjtotffi.html

[R60] 只看 HTTP 状态码
来源：http://hz.chenlongwang.top/gtvbannzlg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gtlrbyxvos.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtqiklxqvc.html

df -h;  du -sh *
来源：http://hz.jyoumei.cn/gtbqffvrsu.html

[R62] 找最占空间的文件
来源：http://hz.hfpthk.cn/gtnovvpegv.html

du -ah . | sort -rh | head -10
来源：http://hz.xuetiantiany.cn/gtoavevivk.html

[R63] 内存与进程
来源：http://hz.yongpay.top/gtypyaqfgk.html

free -h;  ps aux | grep nginx
来源：http://hz.hysaishi.cn/gtbhshmcoz.html

[R64] 结束进程
来源：http://hz.yanxiufei.cn/gtqzjwobsr.html

kill -9 $(pgrep -f app.py)
来源：http://hz.xuanzx.com/gtsiiogewz.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gttnzwijyu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gotoacloud.top/gtxflbfywv.html

[R66] 定时任务
来源：http://hz.cheryme.top/gtfgfbwgfj.html

crontab -e;  crontab -l
来源：http://hz.fzhhl.top/gtluyelcax.html

[R67] 生成随机十六进制串
来源：http://hz.jqgufenzy.top/gtombxjunu.html

openssl rand -hex 16
来源：http://hz.fzhhl.top/gtmkoyjkgm.html

[R68] 计算文件校验值
来源：http://hz.yj20258.top/gtexveozrq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.haohaochexian.top/gtvofygxpt.html

[R69] 生成随机密码
来源：http://hz.guowangkeji.top/gtdzpgjhgx.html

head -c 16 /dev/urandom | base64
来源：http://hz.hywenlv.cn/gtsdyqpavd.html

[R70] 时间戳与互转
来源：http://hz.9152youxi.cn/gtozgsmnkz.html

date +%s;  date -d @1700000000
来源：http://hz.wangshuangyany.cn/gtbdbuifmu.html

[R71] 日期格式化
来源：http://hz.zhaomingkeji.xyz/gtxnkodsbr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.zycfv.cn/gtasxkrzds.html

[R72] 等待端口就绪
来源：http://hz.cqqwz.cn/gtmlwehjgj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.cdnleiting.top/gtpkkjkuan.html

[R73] 分割大日志
来源：http://hz.jyoumei.cn/gtjoduqhbd.html

split -l 1000 big.log part_
来源：http://hz.jinyuanbaomall.cn/gtjyoagicu.html

[R74] 批量重命名
来源：http://hz.gotoacloud.top/gtydhwalfv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hammf.cn/gtcoixclse.html

[R75] 导出环境变量
来源：http://hz.jinyuanbaomall.cn/gtpopyvsrc.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.shanyushiyangtech.top/gtycrbmlpp.html

[R76] 使用临时文件
来源：http://hz.dashuyun.cn/gtfwocuzgy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gtatowwkkc.html

[R77] 读取用户输入
来源：http://hz.jlsjyb.cn/gtvqmqvxrm.html

read -rp "请输入: " ans
来源：http://hz.guannengcc.top/gtvtjjngee.html

[R78] 交互式菜单
来源：http://hz.cashguo.top/gtfetrnyxj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.tianlin.xyz/gtynbttnih.html

[R79] 解析命令行选项
来源：http://hz.xuanzx.com/gtoyfyfodi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.mhx1999.top/gtkrxdzdnn.html

[R80] 查看脚本执行耗时
来源：http://hz.havefunace.top/gteiaubwzg.html

time ./run.sh
来源：http://hz.jinghuilouyu.cn/gtnrbakmgw.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtftvyjacz.html

S. C / C++ 专题
来源：http://hz.gzhubu.top/gtuaavozma.html

================================================================================
来源：http://hz.nwbrower.top/gtpbgtulcn.html

[S01] C：Hello World
来源：http://hz.aibaodan.cn/gtzgibdbiq.html

#include <stdio.h>
来源：http://hz.mhx1999.top/gtxiagvwoh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.cucudq.cn/gtaycnooae.html

[S02] C：变量与格式化输出
来源：http://hz.havefunace.top/gtamjvegoj.html

int a = 10; printf("%d\n", a);
来源：http://hz.zdqjudy.top/gtidmxbukr.html

[S03] C：读入整数
来源：http://hz.andypj.xyz/gtmjxfqduy.html

int x; scanf("%d", &x);
来源：http://hz.yongpay.top/gtaousjtju.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangtech.top/gtizqjcusr.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jinghuilouyu.cn/gtfcignltd.html

[S05] C：字符串长度
来源：http://hz.ybcxt.top/gtoeqypxbe.html

strlen(s)
来源：http://hz.wangshuangyany.cn/gtvfizvczo.html

[S06] C：字符串比较
来源：http://hz.xziqi.cn/gtpzdvwymh.html

strcmp(a, b) == 0
来源：http://hz.gzhubu.top/gtilhmwzmo.html

[S07] C：数组遍历求和
来源：http://hz.0kj1m.cn/gtqskjqkhw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.ybcxt.top/gtjkohslsb.html

[S08] C：动态内存分配与释放
来源：http://hz.yuxming.cn/gtukohfbfd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.guowangkeji.top/gtqkioqvvr.html

[S09] C：结构体定义与初始化
来源：http://hz.0kj1m.cn/gtyvhenlht.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ppjwa.cn/gtgsnsatxb.html

[S10] C：指针与解引用
来源：http://hz.nanxuanxn.top/gtlolljepd.html

int *p = &a;  *p = 5;
来源：http://hz.316326.xyz/gtuzaxyvma.html

[S11] C：逐行读文件
来源：http://hz.xinyue.icu/gtyfewxnys.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.svipenyu.cn/gtpgzsursj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.chenzaomai.com/gtbpckqxvp.html

fclose(f);
来源：http://hz.ehwqpu.com/gtpovysiny.html

[S12] C：写文件
来源：http://hz.zhijiandao.cn/gtqbqpkjel.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.tian-w.cn/gtislzjjmx.html

[S13] C：宏定义
来源：http://hz.cdnleiting.top/gtduuhhwvt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.shzxlz.cn/gtbogqwhse.html

[S14] C：枚举
来源：http://hz.xylfe.cn/gtekzoqyjw.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.hfpthk.cn/gttdgxmwal.html

[S15] C：类型转换
来源：http://hz.xuanzx.com/gtztucwwgf.html

(double) a / b
来源：http://hz.hfpthk.cn/gtjbdaxnhc.html

[S16] C：位操作置位
来源：http://hz.zhoulong.xyz/gtznaqrfzw.html

x |= (1 << 3);
来源：http://hz.sufxvd.cn/gtpiyfcedm.html

[S17] C：安全拼接字符串
来源：http://hz.ywan-chungtsiang.top/gtqgwkaaes.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.guannengcc.top/gtdzsmyqth.html

[S18] C：命令行参数
来源：http://hz.smart0.xyz/gtrtqcdjis.html

int main(int argc, char **argv)
来源：http://hz.yanxiufei.cn/gtmhhzbrfd.html

[S19] C：快速排序
来源：http://hz.jqgfzy.top/gtovmnrefp.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.kuanghao11.cn/gtztpfsmoj.html

[S20] C：二分查找
来源：http://hz.chenjidiqi.icu/gtipurghzw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.xuetiantiany.cn/gttplmagat.html

[S21] C：字符类别判断
来源：http://hz.jianghu66.top/gttphkmslw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.zycfv.cn/gtegtfanlj.html

[S22] C：字符串转数字
来源：http://hz.cucudq.cn/gtrjjscrxs.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xuanzx.com/gtcyvpsksf.html

[S23] C：随机数
来源：http://hz.nwbrower.top/gtnegjdgeb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yj20258888.top/gtatpfldsq.html

[S24] C：获取本地时间
来源：http://hz.cashguo.top/gtdwowquln.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.wangdashe.top/gtvthpenva.html

[S25] C：内存拷贝
来源：http://hz.smart0.xyz/gtthfwjmqj.html

memcpy(dst, src, n);
来源：http://hz.hongshengwenyu.top/gtkurcyvrv.html

[S26] C：内存清零
来源：http://hz.yvedp.cn/gtbyqwwdqt.html

memset(a, 0, sizeof a);
来源：http://hz.yonumen.top/gtdngfybla.html

[S27] C：定义常量
来源：http://hz.svipenyu.cn/gtmeonmjgc.html

const double PI = 3.14159;
来源：http://hz.yj20258.top/gtfmqfajkn.html

[S28] C：静态变量
来源：http://hz.gaohongyu789.top/gtpyynljej.html

static int counter = 0;
来源：http://hz.hammf.cn/gtueanzczm.html

[S29] C：变参函数
来源：http://hz.yangfankeji.com/gtpnvruuhg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ehwqpu.com/gtuvncohmm.html

[S30] C：头文件保护
来源：http://hz.mhx1999.top/gtlmrksyby.html

#ifndef X_H
来源：http://hz.sxryk.cn/gtnedcphmx.html

#define X_H
来源：http://hz.zhengqikj.top/gtqllddqpz.html

#endif
来源：http://hz.ehwqpu.com/gtdgbectpd.html

[S31] C++：Hello World
来源：http://hz.aizwys.cn/gtstvkcavy.html

#include <iostream>
来源：http://hz.tian-w.cn/gtmfpzttxz.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.gzhubu.top/gtnuvxmhxg.html

[S32] C++：字符串
来源：http://hz.ydzc1.top/gtzbbzyynh.html

std::string s = "hi";  s += "!";
来源：http://hz.quarkkingdee.top/gtswiozkts.html

[S33] C++：vector 增删
来源：http://hz.jqgufenzy.top/gtfsgsmguv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.cheryme.top/gthfizhyln.html

[S34] C++：遍历 vector
来源：http://hz.yj20258.top/gtwuemwbqi.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.feifeiyinyue.top/gtpdggvjcx.html

[S35] C++：map
来源：http://hz.zhijiandao.cn/gtojkkhkly.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.vqdsnc.cn/gtcnfaekde.html

[S36] C++：unordered_map
来源：http://hz.birdmap.top/gtnptkjhdo.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.c1oappe.top/gthxlnvjzm.html

[S37] C++：set
来源：http://hz.c1oappe.top/gtcirnjobo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.guannengcc.top/gttidjmhxk.html

[S38] C++：排序
来源：http://hz.jianghu66.top/gtjwbkjkyz.html

std::sort(v.begin(), v.end());
来源：http://hz.xylfe.cn/gtalduesws.html

[S39] C++：自定义比较器排序
来源：http://hz.316326.xyz/gtutizbuse.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.jyoumei.cn/gtfgtofzvn.html

[S40] C++：查找元素
来源：http://hz.haohaochexian.top/gtwgzvxfxe.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.tian-w.cn/gtvwsjlqef.html

[S41] C++：类与构造函数
来源：http://hz.316326.xyz/gtnnodbfuw.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.cheryme.top/gtxfdsvquf.html

[S42] C++：继承与虚函数
来源：http://hz.gzhubu.top/gttdrwgwsv.html

class B : public Base { public: void f() override {} };
来源：http://hz.hongshengwenyu.top/gtpldokwfu.html

[S43] C++：智能指针
来源：http://hz.aibaodan.cn/gtfabewmps.html

auto p = std::make_unique<int>(5);
来源：http://hz.redwolf501.top/gtxrlfmumk.html

[S44] C++：引用传参
来源：http://hz.yangfankeji.com/gtlpwrkfdx.html

void inc(int &x) { ++x; }
来源：http://hz.ydzc1.top/gtbyfwwkpu.html

[S45] C++：lambda
来源：http://hz.bjfxy.top/gtipiiodux.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.zhijiandao.cn/gtbpxwpfac.html

[S46] C++：函数模板
来源：http://hz.cqqwz.cn/gthazfcdjm.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.zhoulong.xyz/gtvxvrcumq.html

[S47] C++：结构化绑定遍历
来源：http://hz.jianghu66.top/gtxddwiuzw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hz.sweek.top/gtiudfhyvz.html

[S48] C++：逐行读文件
来源：http://hz.xuanzx.com/gtnsdousat.html

std::ifstream in("a.txt");  std::string line;
来源：http://hz.gotoacloud.top/gtbisajzwp.html

while (std::getline(in, line)) { }
来源：http://hz.iojbl.cn/gtzgnbwmme.html

[S49] C++：写文件
来源：http://hz.cqqwz.cn/gtsxfbazcj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.zhaomingkeji.xyz/gttxnlyscx.html

[S50] C++：格式化数字
来源：http://hz.cdnleiting.top/gtpzgprijr.html


<!-- 参考信息 -->