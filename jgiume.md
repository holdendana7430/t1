代发 wailian999

[Q76] 按天统计
来源：http://hz.jinyuanbaomall.cn/gtfanunvyt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.chenlongwang.top/gtmevctpco.html

[Q77] 时间加减
来源：http://hz.ybcxt.top/gtfqyypcys.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.9152youxi.cn/gtixmuxjgz.html

[Q78] 当前时间
来源：http://hz.hnqzz.top/gtaqxziuqc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.dianchejie.cn/gtjkmviqry.html

[Q79] 字符串拼接
来源：http://hz.gotoacloud.top/gtjiuxzaqh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.tanke756.top/gtzzigspli.html

[Q80] 字符串截取
来源：http://hz.yvedp.cn/gtgubsrawu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.cdnleiting.top/gtswixmkdj.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtcczjubir.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sufxvd.cn/gtusesevqz.html

[Q82] 字符长度与字节长度
来源：http://hz.hammf.cn/gtrlbkjwgf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.dashuyun.cn/gthkspbvgz.html

[Q83] 大小写转换
来源：http://hz.shanyushiyangkeji.top/gtnfsbbzek.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xuanzx.com/gtgpwvsasw.html

[Q84] 去除首尾空格
来源：http://hz.xuetiantiany.cn/gtiotkhmhs.html

SELECT TRIM(name) FROM users;
来源：http://hz.daria6918.cn/gtimvgfvaf.html

[Q85] 数值取整
来源：http://hz.yvedp.cn/gtepmaklul.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gotoacloud.top/gtuwfhfozt.html

[Q86] 读取 JSON 字段
来源：http://hz.aibaodan.cn/gthymfzupl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.smart0.xyz/gtlwlltmqo.html

[Q87] JSON 字段做条件
来源：http://hz.jinqigufen.top/gtjqwpyzwk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gtthzsobdf.html

[Q88] 行转列（条件聚合）
来源：http://hz.hnqzz.top/gtstmurpxt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.dashuyun.cn/gttjqpmljf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.sweek.top/gtzghjrsnv.html

[Q89] 判断表是否存在
来源：http://hz.sweek.top/gtmzxpkanf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.jianghu66.top/gttrzxqsgo.html

[Q90] 生成序号列
来源：http://hz.zhengqikj.top/gtzikezenb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtnrlasgil.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtmyyhmpzc.html

R. Bash 专题
来源：http://hz.ppjwa.cn/gtxudmhesy.html

================================================================================
来源：http://hz.guowangkeji.top/gtuzctvbuy.html

[R01] shebang 与严格模式
来源：http://hz.yanxiufei.cn/gtznnzjrpe.html

#!/usr/bin/env bash
来源：http://hz.tanke756.top/gtavrlpkht.html

set -euo pipefail
来源：http://hz.yj20258.top/gtsgbhwjij.html

[R02] 变量赋值与使用
来源：http://hz.tianlin.xyz/gtndwbdino.html

name="Tom"; echo "$name"
来源：http://hz.hnqzz.top/gtfyujjzqc.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtnwmcmykp.html

readonly PI=3.14
来源：http://hz.zhongyouzk.top/gtossvzjwy.html

[R04] 位置参数
来源：http://hz.smart0.xyz/gtwmfhhwru.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhoulong.xyz/gtgkhatslj.html

[R05] 参数默认值
来源：http://hz.tianlin.xyz/gttnugbvkd.html

name="${1:-default}"
来源：http://hz.iojbl.cn/gtwunhszad.html

[R06] 判断命令是否存在
来源：http://hz.yanxiufei.cn/gtulggdfys.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yangfankeji.com/gtrxubqxyq.html

[R07] if 判断文件
来源：http://hz.yangfankeji.com/gtpdscnnra.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.pycfn.com/gtiiytvpbj.html

[R08] 数值比较
来源：http://hz.mhx1999.top/gtkoxwamlm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.ivvv.top/gtrnidmfbh.html

[R09] 字符串比较
来源：http://hz.jinqigufen.top/gttlvzytob.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.meibo888.top/gtjnukrxuj.html

[R10] 正则匹配
来源：http://hz.jlsjyb.cn/gtcmpcmsus.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.guannengcc.top/gtxvktyhnh.html

[R11] case 多分支
来源：http://hz.sysykeji.top/gtnyqwoqgk.html

case "$1" in
来源：http://hz.cashguo.top/gtfmrtigfu.html

start) echo "启动" ;;
来源：http://hz.meibo888.top/gtqrxxpnbc.html

stop)  echo "停止" ;;
来源：http://hz.cucudq.cn/gtrvuzupht.html

*)     echo "未知命令" ;;
来源：http://hz.yueranfly.top/gtdrezutkc.html

esac
来源：http://hz.jyoumei.cn/gtxqptixsj.html

[R12] for 遍历文件
来源：http://hz.guannengcc.top/gtkxfdqbnj.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtyqdvrmoe.html

[R13] for 计数循环
来源：http://hz.yvedp.cn/gtvhksanat.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fengsongda.top/gtfmvftmaj.html

[R14] C 风格 for
来源：http://hz.zhongyouzk.top/gtmllhgxhw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.gaohongyu789.top/gtbjovxeur.html

[R15] while 逐行读文件
来源：http://hz.quarkkingdee.top/gthnhcjzft.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.yuanzhike.top/gtrjyuqfnq.html

[R16] until 等待条件
来源：http://hz.ivvv.top/gtxwbtryof.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.hammf.cn/gtsvyciicq.html

[R17] 数组定义与取值
来源：http://hz.jinyuanbaomall.cn/gtuoiwyocp.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.quarkkingdee.top/gtovxfaadv.html

[R18] 遍历数组
来源：http://hz.haohaochexian.top/gtjqlqqvvi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.tanke756.top/gtvranycie.html

[R19] 数组长度
来源：http://hz.wangdashe.top/gtzjyyurts.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtcmhwrumu.html

[R20] 关联数组（字典）
来源：http://hz.guowangkeji.top/gtybzxpobw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ywan-chungtsiang.top/gttrrfeixc.html

[R21] 字符串长度
来源：http://hz.fzhhl.top/gtsezlxwxs.html

echo "${#s}"
来源：http://hz.birdmap.top/gtxybwgpoc.html

[R22] 截取子串
来源：http://hz.52xcode.cn/gtxewucjsj.html

echo "${s:0:5}"
来源：http://hz.hywenlv.cn/gtjpyxqpon.html

[R23] 字符串替换
来源：http://hz.gaohongyu789.top/gtxvaciryo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.nwbrower.top/gtaqezykml.html

[R24] 大小写转换
来源：http://hz.fengsongda.top/gtqqqobhpw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.0kj1m.cn/gtfywhkkpm.html

[R25] 去后缀 / 去前缀
来源：http://hz.zdqjudy.top/gthxoveqxc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.guannengcc.top/gtysgtekcp.html

[R26] 命令替换
来源：http://hz.shzxlz.cn/gtysozanrw.html

now=$(date +%F); echo "$now"
来源：http://hz.hfpthk.cn/gtfxtmypok.html

[R27] 算术展开
来源：http://hz.hfpthk.cn/gtnmzkbksu.html

echo $((1 + 2 * 3))
来源：http://hz.pengpengdd.cyou/gtpbefuoxm.html

[R28] 浮点运算
来源：http://hz.guannengcc.top/gtggnqkhpa.html

echo "scale=2; 10/3" | bc
来源：http://hz.aibaodan.cn/gtphioyyvu.html

[R29] 定义函数
来源：http://hz.wangdashe.top/gttwwmpals.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.aibaodan.cn/gtnzcmnqdx.html

[R30] 函数返回状态码
来源：http://hz.ehwqpu.com/gtpxiavncv.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj202588.top/gtddmcyjgb.html

[R31] 局部变量
来源：http://hz.kuanghao11.cn/gtnsvyrvdj.html

f() { local x=1; echo "$x"; }
来源：http://hz.havefunace.top/gtklulnxot.html

[R32] 参数个数校验
来源：http://hz.iojbl.cn/gtefiuztni.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.shzxlz.cn/gtrfopdccr.html

[R33] 捕获错误并提示行号
来源：http://hz.shzxlz.cn/gtvbuigdeb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuetiantiany.cn/gtyxkxblkm.html

[R34] 退出时清理
来源：http://hz.redwolf501.top/gtdgcpgudx.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.sxryk.cn/gtzvbpqumh.html

[R35] 后台执行并等待
来源：http://hz.shanyushiyangkeji.top/gtjjkjgapr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ivvv.top/gtxvzmzhqw.html

[R36] 并发执行多个任务
来源：http://hz.jqgfzy.top/gtqkykzhog.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtfxzmgrto.html

[R37] 把输出赋给变量
来源：http://hz.dianchejie.cn/gtjccuxmom.html

files=$(ls -1)
来源：http://hz.daria6918.cn/gtirtcpdkw.html

[R38] 管道串联
来源：http://hz.wangdashe.top/gtbbyyjynt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.havefunace.top/gtsopkqrzi.html

[R39] 重定向标准输出与错误
来源：http://hz.birdmap.top/gtksxahjls.html

cmd > out.log 2>&1
来源：http://hz.jinyuanbaomall.cn/gtfkevtedo.html

[R40] 追加写日志
来源：http://hz.iojbl.cn/gtklurjkdw.html

echo "log" >> out.log
来源：http://hz.dashuyun.cn/gtusnzqqyg.html

[R41] 丢弃输出
来源：http://hz.cqqwz.cn/gtsddkdbno.html

cmd >/dev/null 2>&1
来源：http://hz.shzxlz.cn/gtidvlkkqp.html

[R42] 输入重定向
来源：http://hz.zhixingplan.top/gttxfjiuvd.html

wc -l < a.txt
来源：http://hz.xingfuxueyuan.xyz/gthagzreas.html

[R43] 按名字查找文件
来源：http://hz.feifeiyinyue.top/gtaxvderxb.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gtybxbllhe.html

[R44] 按修改时间查找
来源：http://hz.snrcjt.cn/gtgurqiwzl.html

find . -mtime -7 -type f
来源：http://hz.yongpay.top/gtvpvxxkfc.html

[R45] 批量删除
来源：http://hz.yj202588.top/gtbresiugk.html

find . -name "*.tmp" -delete
来源：http://hz.kuanghao11.cn/gtadbyjmif.html

[R46] 递归替换文件内容
来源：http://hz.cashguo.top/gtnhfxrjly.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.guowangkeji.top/gtjdtftuku.html

[R47] sed 单行替换
来源：http://hz.jqgufenzy.top/gtkdkexabw.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gthyxrmsuv.html

[R48] awk 取指定列
来源：http://hz.jqgfzy.top/gtxbuajxaa.html

awk '{print $1, $3}' a.txt
来源：http://hz.pycfn.com/gtwmccdkvi.html

[R49] awk 带条件
来源：http://hz.iojbl.cn/gtarxbiggf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shuidangran.top/gtxfxtftif.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtggppotes.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.cqqwz.cn/gtbmivppmf.html

[R51] 排序去重取前几
来源：http://hz.cheryme.top/gtpxayqhlw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.quarkkingdee.top/gtqnppayir.html

[R52] 统计行数
来源：http://hz.ydjk.org.cn/gtdbklulkr.html

wc -l a.txt
来源：http://hz.quarkkingdee.top/gtdhcpdqfg.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtursskifv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtcatbuvsh.html

[R54] 比较两个文件
来源：http://hz.c1oappe.top/gtmszinpzl.html

diff a.txt b.txt
来源：http://hz.sxryk.cn/gtbuyhsnzh.html

[R55] 压缩与解压
来源：http://hz.shangyingyoupin.top/gtsyfjlnzi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.cashguo.top/gtnkrtjgbb.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtxejbxcpg.html

scp file user@host:/path/
来源：http://hz.yanxiufei.cn/gtsgvmauqm.html

[R57] 远程执行命令
来源：http://hz.tianlin.xyz/gtxgdhsnnq.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gtswbhklqk.html

[R58] 下载文件
来源：http://hz.nanxinkj.top/gtizqrkcmg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.daria6918.cn/gtdddhtjge.html

[R59] 发 POST JSON
来源：http://hz.52xcode.cn/gtuwrviuze.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.ivvv.top/gtscgjlolg.html

[R60] 只看 HTTP 状态码
来源：http://hz.cheryme.top/gtqhizdqfe.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.tian-w.cn/gtxgwddcmu.html

[R61] 磁盘占用
来源：http://hz.hfpthk.cn/gtiwcverat.html

df -h;  du -sh *
来源：http://hz.redwolf501.top/gtpcamgyak.html

[R62] 找最占空间的文件
来源：http://hz.gogol.net.cn/gtmwnwevgs.html

du -ah . | sort -rh | head -10
来源：http://hz.quarkkingdee.top/gtrdcdzohi.html

[R63] 内存与进程
来源：http://hz.chenlongwang.top/gtndvodbja.html

free -h;  ps aux | grep nginx
来源：http://hz.shanyushiyangtech.top/gtzmvybfyl.html

[R64] 结束进程
来源：http://hz.gaohongyu789.top/gtposqwhop.html

kill -9 $(pgrep -f app.py)
来源：http://hz.fzhhl.top/gtxspojata.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtkqoxdiba.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.birdmap.top/gtczgowean.html

[R66] 定时任务
来源：http://hz.fengsongda.top/gttdifeybt.html

crontab -e;  crontab -l
来源：http://hz.ivvv.top/gtsahputvc.html

[R67] 生成随机十六进制串
来源：http://hz.tianlin.xyz/gtlbwzqvhs.html

openssl rand -hex 16
来源：http://hz.andypj.xyz/gtwpiydhfe.html

[R68] 计算文件校验值
来源：http://hz.tian-w.cn/gttlymrvnx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhijiandao.cn/gtoaaqhwax.html

[R69] 生成随机密码
来源：http://hz.mhx1999.top/gtghuxlkcf.html

head -c 16 /dev/urandom | base64
来源：http://hz.9152youxi.cn/gtpjhotffo.html

[R70] 时间戳与互转
来源：http://hz.jqgufenzy.top/gtckaxmzgj.html

date +%s;  date -d @1700000000
来源：http://hz.bjfxy.top/gthkofuycu.html

[R71] 日期格式化
来源：http://hz.c1oappe.top/gtsmtpunff.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.aizwys.cn/gttwxaoncn.html

[R72] 等待端口就绪
来源：http://hz.hnxiangtu.top/gtqsaajopn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtixusntzc.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtaupyekwp.html

split -l 1000 big.log part_
来源：http://hz.yuanzhike.top/gttsocwmvy.html

[R74] 批量重命名
来源：http://hz.yuxming.cn/gtjhovivnv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gtoolqhwzk.html

[R75] 导出环境变量
来源：http://hz.aibaodan.cn/gtvarycqoy.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yueranfly.top/gtirgchpcx.html

[R76] 使用临时文件
来源：http://hz.tanke756.top/gtpumyxced.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jyoumei.cn/gtljsoltax.html

[R77] 读取用户输入
来源：http://hz.nanxuanxn.top/gtihywdskj.html

read -rp "请输入: " ans
来源：http://hz.cheryme.top/gtwuqawhzo.html

[R78] 交互式菜单
来源：http://hz.hongshengwenyu.top/gtipvpfjdb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhoulong.xyz/gtkyzpavjr.html

[R79] 解析命令行选项
来源：http://hz.guannengcc.top/gtzzrciybu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jinyuanbaomall.cn/gtvxtyafzz.html

[R80] 查看脚本执行耗时
来源：http://hz.xylfe.cn/gtymibubwk.html

time ./run.sh
来源：http://hz.yj20258888.top/gthbpzjies.html

================================================================================
来源：http://hz.bjfxy.top/gtyxdogeym.html

S. C / C++ 专题
来源：http://hz.pengpengdd.cyou/gtqdpqkrre.html

================================================================================
来源：http://hz.c1oappe.top/gtxqgvpzne.html

[S01] C：Hello World
来源：http://hz.cashguo.top/gtypqwulzk.html

#include <stdio.h>
来源：http://hz.tian-w.cn/gtdlabqboh.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.9152youxi.cn/gtlkwbdxpu.html

[S02] C：变量与格式化输出
来源：http://hz.mhx1999.top/gtclcllgty.html

int a = 10; printf("%d\n", a);
来源：http://hz.shangyingyoupin.top/gtobftfnpk.html

[S03] C：读入整数
来源：http://hz.fengsongda.top/gtctgfvbec.html

int x; scanf("%d", &x);
来源：http://hz.hnxiangtu.top/gtrdyriczv.html

[S04] C：字符串复制
来源：http://hz.snrcjt.cn/gtfqdifzsu.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yj20258888.top/gtrlnbbnkb.html

[S05] C：字符串长度
来源：http://hz.yj202588.top/gttzfgmnez.html

strlen(s)
来源：http://hz.zhiwuduotai.top/gtpzbrtzww.html

[S06] C：字符串比较
来源：http://hz.zhengqikj.top/gteicieebo.html

strcmp(a, b) == 0
来源：http://hz.smart0.xyz/gtyaacvrhu.html

[S07] C：数组遍历求和
来源：http://hz.feifeiyinyue.top/gtldietuwc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.kuanghao11.cn/gtvzkzwyeh.html

[S08] C：动态内存分配与释放
来源：http://hz.c1oappe.top/gtgymthrwe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yongpay.top/gtdxecdnij.html

[S09] C：结构体定义与初始化
来源：http://hz.meibo888.top/gtwaknvpjq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.dianchejie.cn/gtinywqcjl.html

[S10] C：指针与解引用
来源：http://hz.wangshuangyany.cn/gtiizhourk.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtujqqnwlu.html

[S11] C：逐行读文件
来源：http://hz.yj20258.top/gtsjihjyzl.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jqgfzy.top/gtdozxvrao.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.tianlin.xyz/gtkpffiwcx.html

fclose(f);
来源：http://hz.zhijiandao.cn/gtmqxnlybg.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtdjrcaqpz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.fengsongda.top/gtfamtrawa.html

[S13] C：宏定义
来源：http://hz.yuanzhike.top/gtorpjqxog.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.hnxiangtu.top/gtevpztdwn.html

[S14] C：枚举
来源：http://hz.andypj.xyz/gtmychneoc.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.cheryme.top/gtbroqagwd.html

[S15] C：类型转换
来源：http://hz.fzhhl.top/gtengcuhms.html

(double) a / b
来源：http://hz.hfpthk.cn/gtvnbpjtuz.html

[S16] C：位操作置位
来源：http://hz.jinghuilouyu.cn/gtwsxtgzqz.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtupyifhbn.html

[S17] C：安全拼接字符串
来源：http://hz.andypj.xyz/gtcgtmbqub.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ivvv.top/gtbdmqeokh.html

[S18] C：命令行参数
来源：http://hz.zhixingplan.top/gtjuodzrtx.html

int main(int argc, char **argv)
来源：http://hz.gaohongyu789.top/gtdzzgnqfd.html

[S19] C：快速排序
来源：http://hz.ywan-chungtsiang.top/gtacvghlua.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.yanxiufei.cn/gtbilzehbu.html

[S20] C：二分查找
来源：http://hz.snrcjt.cn/gtptesghpe.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hysaishi.cn/gtexbunwqu.html

[S21] C：字符类别判断
来源：http://hz.jlsjyb.cn/gtpksoexss.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.xziqi.cn/gtlvyzrxmk.html

[S22] C：字符串转数字
来源：http://hz.meibo888.top/gtkpraunor.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.zhixingplan.top/gthefsjmvt.html

[S23] C：随机数
来源：http://hz.ehwqpu.com/gteifombwo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.fengsongda.top/gthcmrkthp.html

[S24] C：获取本地时间
来源：http://hz.yueranfly.top/gtmxokhqpm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yvedp.cn/gtsswxpyzy.html

[S25] C：内存拷贝
来源：http://hz.daria6918.cn/gtjncxuhch.html

memcpy(dst, src, n);
来源：http://hz.feifeiyinyue.top/gtfjmghjrm.html

[S26] C：内存清零
来源：http://hz.zdqjudy.top/gtjvrsyenk.html

memset(a, 0, sizeof a);
来源：http://hz.havefunace.top/gtsggjxwlk.html

[S27] C：定义常量
来源：http://hz.xylfe.cn/gtiiolcxqn.html

const double PI = 3.14159;
来源：http://hz.cashguo.top/gtyvotuveu.html

[S28] C：静态变量
来源：http://hz.chenlongwang.top/gtexfhkbwr.html

static int counter = 0;
来源：http://hz.zhongyouzk.top/gtkcevkmjh.html

[S29] C：变参函数
来源：http://hz.0kj1m.cn/gtibedimdl.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.gaohongyu789.top/gtqxyvewor.html

[S30] C：头文件保护
来源：http://hz.yj202588.top/gtjwfljfol.html

#ifndef X_H
来源：http://hz.shanyushiyangkeji.top/gtrzommklv.html

#define X_H
来源：http://hz.quarkkingdee.top/gtzlqspgzz.html

#endif
来源：http://hz.guannengcc.top/gtsnyhiezx.html

[S31] C++：Hello World
来源：http://hz.daria6918.cn/gtwpsqnkfl.html

#include <iostream>
来源：http://hz.jyoumei.cn/gthuvhsbqt.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.yuxming.cn/gtedetlkep.html

[S32] C++：字符串
来源：http://hz.zhoulong.xyz/gttpsljtpd.html

std::string s = "hi";  s += "!";
来源：http://hz.sufxvd.cn/gtemxlqzaa.html

[S33] C++：vector 增删
来源：http://hz.meibo888.top/gttozdpygz.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.yueranfly.top/gtudtoguzj.html

[S34] C++：遍历 vector
来源：http://hz.hnqzz.top/gtiaohpahq.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.316326.xyz/gtmgxnxiqg.html

[S35] C++：map
来源：http://hz.fzhhl.top/gtvfzemdgt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.sxryk.cn/gtqgfliknp.html

[S36] C++：unordered_map
来源：http://hz.ivvv.top/gtbcymomdc.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.dianchejie.cn/gtyhhiutvh.html

[S37] C++：set
来源：http://hz.tian-w.cn/gtcpipypoy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hz.sufxvd.cn/gtmdjucqyo.html

[S38] C++：排序
来源：http://hz.0kj1m.cn/gtebggifsu.html

std::sort(v.begin(), v.end());
来源：http://hz.tanke756.top/gtisnylgkp.html

[S39] C++：自定义比较器排序
来源：http://hz.wangdashe.top/gthrbtpddd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hz.xingfuxueyuan.xyz/gtwepxqqln.html

[S40] C++：查找元素
来源：http://hz.zhongyouzk.top/gtosritnug.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hz.pycfn.com/gtmsbztcqd.html

[S41] C++：类与构造函数
来源：http://hz.jqgfzy.top/gtualrwjte.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hz.yanxiufei.cn/gticjlfwwf.html

[S42] C++：继承与虚函数
来源：http://hz.jinyuanbaomall.cn/gtxvhrkadr.html

class B : public Base { public: void f() override {} };
来源：http://hz.0kj1m.cn/gtboqcysuh.html

[S43] C++：智能指针
来源：http://hz.gzhubu.top/gtcpaxjeau.html

auto p = std::make_unique<int>(5);
来源：http://hz.hysaishi.cn/gtfbaqcbhm.html

[S44] C++：引用传参
来源：http://hz.fengsongda.top/gtymschlth.html

void inc(int &x) { ++x; }
来源：http://hz.ybcxt.top/gtrequhceb.html

[S45] C++：lambda
来源：http://hz.c1oappe.top/gthtnewgng.html

auto add = [](int a, int b) { return a + b; };
来源：http://hz.cucudq.cn/gtzttrmglt.html

[S46] C++：函数模板
来源：http://hz.zhoulong.xyz/gtyjmvvlol.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hz.hfpthk.cn/gtwujsqrww.html


<!-- 参考信息 -->