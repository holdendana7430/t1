代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.jinqigufen.top/gtnjzhpjof.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.gaohongyu789.top/gtbfetmmff.html

[Q68] 保存点
来源：http://hz.zhoulong.xyz/gtbmrvzizs.html

SAVEPOINT sp1;
来源：http://hz.0kj1m.cn/gtogvusczp.html

ROLLBACK TO sp1;
来源：http://hz.yj202588.top/gthzsuqwrd.html

[Q69] 查看执行计划
来源：http://hz.pengpengdd.cyou/gthswgzwcp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.xuanzx.com/gtlyxryiil.html

[Q70] 更新统计信息
来源：http://hz.aizwys.cn/gtdcvxsfde.html

ANALYZE TABLE users;
来源：http://hz.sufxvd.cn/gtvjgzghjo.html

[Q71] 查看建表语句
来源：http://hz.jlsjyb.cn/gtctnosakb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.chenjidiqi.icu/gtupblyigl.html

[Q72] 查看索引
来源：http://hz.fzhhl.top/gtlhrfohsf.html

SHOW INDEX FROM users;
来源：http://hz.jlsjyb.cn/gtsqwlkzdq.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtsqkvjabo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.fengsongda.top/gtziocrqoy.html

[Q74] 强制使用索引
来源：http://hz.jianghu66.top/gtjphupnpw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yangfankeji.com/gtxjlpgale.html

[Q75] 日期格式化
来源：http://hz.svipenyu.cn/gtgnwqinhw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.gotoacloud.top/gtvhgiufaq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.cheryme.top/gtokwakrfu.html

[Q76] 按天统计
来源：http://hz.shzxlz.cn/gtkgvrxtrp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.kuanghao11.cn/gtvxxvxodk.html

[Q77] 时间加减
来源：http://hz.yj20258.top/gtcaqaubff.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nanxinkj.top/gtbpritbrw.html

[Q78] 当前时间
来源：http://hz.yongpay.top/gtlawpexok.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gogol.net.cn/gtkrbognqn.html

[Q79] 字符串拼接
来源：http://hz.fengsongda.top/gtnbbdodkw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yuxming.cn/gtvxddebrj.html

[Q80] 字符串截取
来源：http://hz.shangyingyoupin.top/gtalkxeasr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.ydjk.org.cn/gthiupsyla.html

[Q81] 字符串替换
来源：http://hz.xylfe.cn/gtiuemfxbi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.tianlin.xyz/gtogaapnen.html

[Q82] 字符长度与字节长度
来源：http://hz.hnxiangtu.top/gtzkgbubzc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.shanyushiyangkeji.top/gtlsxeoynv.html

[Q83] 大小写转换
来源：http://hz.daxiang520.top/gtcqwiiwgd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.ydzc1.top/gtwhkokinr.html

[Q84] 去除首尾空格
来源：http://hz.meibo888.top/gtydvhfrrt.html

SELECT TRIM(name) FROM users;
来源：http://hz.guannengcc.top/gtajbhdzww.html

[Q85] 数值取整
来源：http://hz.tanke756.top/gtxxunculu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.zhixingplan.top/gtciwzemuq.html

[Q86] 读取 JSON 字段
来源：http://hz.zhoulong.xyz/gtpzvujbbf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.xinyue.icu/gtuxkebkob.html

[Q87] JSON 字段做条件
来源：http://hz.nanxuanxn.top/gtpshtauwm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.yonumen.top/gtcilyfxtp.html

[Q88] 行转列（条件聚合）
来源：http://hz.wangshuangyany.cn/gtzhjzdvcb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.zhengqikj.top/gttuplgbbb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.iojbl.cn/gtdnzivufs.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtsvhotxoq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.dashuyun.cn/gttdrglviw.html

[Q90] 生成序号列
来源：http://hz.wangdashe.top/gtpbtnpiln.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.shanyushiyangkeji.top/gtrdjjwpof.html

================================================================================
来源：http://hz.xinyue.icu/gtsaaoucfg.html

R. Bash 专题
来源：http://hz.52xcode.cn/gtqtfahnnq.html

================================================================================
来源：http://hz.zdqjudy.top/gttbmhgndy.html

[R01] shebang 与严格模式
来源：http://hz.zhiwuduotai.top/gtaurcawar.html

#!/usr/bin/env bash
来源：http://hz.svipenyu.cn/gtfpfvhqsa.html

set -euo pipefail
来源：http://hz.aibaodan.cn/gtfbwrutme.html

[R02] 变量赋值与使用
来源：http://hz.shanyushiyangkeji.top/gtysihdrgv.html

name="Tom"; echo "$name"
来源：http://hz.zhongyouzk.top/gtgqykcftq.html

[R03] 只读变量
来源：http://hz.smart0.xyz/gtxlcrcwoz.html

readonly PI=3.14
来源：http://hz.yvedp.cn/gtsrdujbwh.html

[R04] 位置参数
来源：http://hz.ivvv.top/gtasaktdzz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.shzxlz.cn/gtmrbnnjls.html

[R05] 参数默认值
来源：http://hz.gaohongyu789.top/gtrnuwuytl.html

name="${1:-default}"
来源：http://hz.hnqzz.top/gtheenwplm.html

[R06] 判断命令是否存在
来源：http://hz.52xcode.cn/gtuuihijjn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.jianghu66.top/gteocetdfj.html

[R07] if 判断文件
来源：http://hz.guannengcc.top/gtxcfuurza.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhengqikj.top/gtocqheiqq.html

[R08] 数值比较
来源：http://hz.shuidangran.top/gtwakrmzyj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.daria6918.cn/gtgweohfzk.html

[R09] 字符串比较
来源：http://hz.daxiang520.top/gtxjlncbgy.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.vqdsnc.cn/gttulextvq.html

[R10] 正则匹配
来源：http://hz.zhijiandao.cn/gtqabmpzbk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yangfankeji.com/gtvsmavevs.html

[R11] case 多分支
来源：http://hz.jinqigufen.top/gtynfvnofk.html

case "$1" in
来源：http://hz.cqqwz.cn/gtkutjzpit.html

start) echo "启动" ;;
来源：http://hz.cheryme.top/gtjidquevf.html

stop)  echo "停止" ;;
来源：http://hz.jinqigufen.top/gtirvxsccf.html

*)     echo "未知命令" ;;
来源：http://hz.haohaochexian.top/gtskupqhge.html

esac
来源：http://hz.daxiang520.top/gtuckrvupm.html

[R12] for 遍历文件
来源：http://hz.sweek.top/gthlylpnkd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhixingplan.top/gtvlndzjsd.html

[R13] for 计数循环
来源：http://hz.0kj1m.cn/gtkseplhyp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.aizwys.cn/gtxrdqfzxe.html

[R14] C 风格 for
来源：http://hz.gogol.net.cn/gtubbmprqc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.jinqigfzy.top/gtrhdtypgh.html

[R15] while 逐行读文件
来源：http://hz.tianlin.xyz/gtkdrocksq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xinyue.icu/gtpwkaiclm.html

[R16] until 等待条件
来源：http://hz.yueranfly.top/gtxgifmwrw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sysykeji.top/gtckebkkfh.html

[R17] 数组定义与取值
来源：http://hz.zycfv.cn/gtfytqlevx.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.sysykeji.top/gtptzbtokd.html

[R18] 遍历数组
来源：http://hz.jianghu66.top/gtzwxyvtpb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhixingplan.top/gtlbuhnfis.html

[R19] 数组长度
来源：http://hz.yvedp.cn/gtrawjmftg.html

echo "${#arr[@]}"
来源：http://hz.feifeiyinyue.top/gtyigqdtnu.html

[R20] 关联数组（字典）
来源：http://hz.redwolf501.top/gtyzpqgfrl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.yonumen.top/gtkcinjjrk.html

[R21] 字符串长度
来源：http://hz.shanyushiyangtech.top/gtlteotxqe.html

echo "${#s}"
来源：http://hz.yueranfly.top/gtzfawtdpq.html

[R22] 截取子串
来源：http://hz.chenlongwang.top/gtwfrbsgxv.html

echo "${s:0:5}"
来源：http://hz.quarkkingdee.top/gteetiftrp.html

[R23] 字符串替换
来源：http://hz.aizwys.cn/gtvgnugyvy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.yj20258888.top/gttxggnemn.html

[R24] 大小写转换
来源：http://hz.birdmap.top/gtzxrwkmde.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cashguo.top/gtvetekvpk.html

[R25] 去后缀 / 去前缀
来源：http://hz.birdmap.top/gtclkizntr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.haohaochexian.top/gtdgvedvnp.html

[R26] 命令替换
来源：http://hz.fzhhl.top/gtkgvwrrcz.html

now=$(date +%F); echo "$now"
来源：http://hz.zhixingplan.top/gtvxzscivd.html

[R27] 算术展开
来源：http://hz.316326.xyz/gtkdrwdknc.html

echo $((1 + 2 * 3))
来源：http://hz.hysaishi.cn/gtxjgodfjf.html

[R28] 浮点运算
来源：http://hz.yueranfly.top/gthietnlhc.html

echo "scale=2; 10/3" | bc
来源：http://hz.cqqwz.cn/gtsbothvbm.html

[R29] 定义函数
来源：http://hz.yuxming.cn/gtimvciaoc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.hysaishi.cn/gtrsbfbkui.html

[R30] 函数返回状态码
来源：http://hz.aibaodan.cn/gtdevzzfte.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jiagoushi.top/gtjhzzyagx.html

[R31] 局部变量
来源：http://hz.jianghu66.top/gthyqrlkzi.html

f() { local x=1; echo "$x"; }
来源：http://hz.hysaishi.cn/gtlygyppqi.html

[R32] 参数个数校验
来源：http://hz.zhaomingkeji.xyz/gtqxcemjzd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.ivvv.top/gtrxeygaxh.html

[R33] 捕获错误并提示行号
来源：http://hz.gaohongyu789.top/gtwhvbfgag.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.xuanzx.com/gtoxrvxzty.html

[R34] 退出时清理
来源：http://hz.hongshengwenyu.top/gtxyudfnqk.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yongpay.top/gtncsgmxno.html

[R35] 后台执行并等待
来源：http://hz.yj20258.top/gtvjyhlbxq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.shanyushiyangkeji.top/gtqhazqnsf.html

[R36] 并发执行多个任务
来源：http://hz.xuetiantiany.cn/gtuiimlluh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.dashuyun.cn/gtxqcmwynn.html

[R37] 把输出赋给变量
来源：http://hz.vqdsnc.cn/gtwueclrbq.html

files=$(ls -1)
来源：http://hz.aibaodan.cn/gtybcsmzur.html

[R38] 管道串联
来源：http://hz.hnqzz.top/gtorntqbsu.html

cat a.txt | grep -i error | wc -l
来源：http://hz.nanxuanxn.top/gtgeygcvds.html

[R39] 重定向标准输出与错误
来源：http://hz.hysaishi.cn/gtdebmyqem.html

cmd > out.log 2>&1
来源：http://hz.yuxming.cn/gtumpmqlof.html

[R40] 追加写日志
来源：http://hz.yvedp.cn/gtsijppkiv.html

echo "log" >> out.log
来源：http://hz.9152youxi.cn/gtnjyhzfqb.html

[R41] 丢弃输出
来源：http://hz.iojbl.cn/gtpjvwndwg.html

cmd >/dev/null 2>&1
来源：http://hz.hnxiangtu.top/gtuoxdqszj.html

[R42] 输入重定向
来源：http://hz.chenlongwang.top/gtidmckkvy.html

wc -l < a.txt
来源：http://hz.jianghu66.top/gtdbrvathm.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtmoklulqi.html

find . -name "*.log" -type f
来源：http://hz.shangyingyoupin.top/gtppqzvowz.html

[R44] 按修改时间查找
来源：http://hz.chenzaomai.com/gtzaqpaaad.html

find . -mtime -7 -type f
来源：http://hz.redwolf501.top/gtmdkedgwx.html

[R45] 批量删除
来源：http://hz.hnxiangtu.top/gtovrjojlg.html

find . -name "*.tmp" -delete
来源：http://hz.yanxiufei.cn/gtxorfuwjf.html

[R46] 递归替换文件内容
来源：http://hz.hammf.cn/gtdnkyyemt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.cheryme.top/gtnjkjpjms.html

[R47] sed 单行替换
来源：http://hz.daria6918.cn/gtzsnrasmj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.haohaochexian.top/gtmmegomgp.html

[R48] awk 取指定列
来源：http://hz.nanxuanxn.top/gtoaufucud.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gttvhflkqr.html

[R49] awk 带条件
来源：http://hz.zdqjudy.top/gtdqtntgva.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtqxaxnvka.html

[R50] awk 求和
来源：http://hz.zhijiandao.cn/gtnnqpxzdg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.tian-w.cn/gttxnajkgd.html

[R51] 排序去重取前几
来源：http://hz.ywan-chungtsiang.top/gtzhgirguv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.gotoacloud.top/gtyvjlfgwx.html

[R52] 统计行数
来源：http://hz.guannengcc.top/gtmwqvhsdr.html

wc -l a.txt
来源：http://hz.wangdashe.top/gtmwpnsumd.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtvdsjqyiv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.gogol.net.cn/gtpgmnsojr.html

[R54] 比较两个文件
来源：http://hz.yongpay.top/gtoalyvbkg.html

diff a.txt b.txt
来源：http://hz.nanxuanxn.top/gtnyuiipbc.html

[R55] 压缩与解压
来源：http://hz.meibo888.top/gtfqvzcies.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.redwolf501.top/gtxeikqyjx.html

[R56] 远程拷贝
来源：http://hz.xuanzx.com/gtnnwpyjjg.html

scp file user@host:/path/
来源：http://hz.zycfv.cn/gtqjwikjaz.html

[R57] 远程执行命令
来源：http://hz.snrcjt.cn/gtvqkpwxox.html

ssh user@host 'uptime'
来源：http://hz.yvedp.cn/gtloukvcfb.html

[R58] 下载文件
来源：http://hz.shanyushiyangtech.top/gtsisrrylp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.meibo888.top/gtooyfqaec.html

[R59] 发 POST JSON
来源：http://hz.meibo888.top/gtitvtxfro.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pycfn.com/gtbnbookfo.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhoulong.xyz/gtmouwohpc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.gotoacloud.top/gtaicupkfw.html

[R61] 磁盘占用
来源：http://hz.chenjidiqi.icu/gtteepkbyp.html

df -h;  du -sh *
来源：http://hz.yueranfly.top/gtpwspeggs.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtxoefrpem.html

du -ah . | sort -rh | head -10
来源：http://hz.gogol.net.cn/gttinzzaaj.html

[R63] 内存与进程
来源：http://hz.zhixingplan.top/gtevrxyikx.html

free -h;  ps aux | grep nginx
来源：http://hz.zhongyouzk.top/gtkxwqaupi.html

[R64] 结束进程
来源：http://hz.shanyushiyangkeji.top/gtgpglvetp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.wangshuangyany.cn/gthngjfvfi.html

[R65] 查看端口占用
来源：http://hz.fengsongda.top/gtlzrchhtt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tian-w.cn/gtdwrkmhai.html

[R66] 定时任务
来源：http://hz.chenlongwang.top/gtbxtiyzmm.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gtrzcuymvb.html

[R67] 生成随机十六进制串
来源：http://hz.jinghuilouyu.cn/gtwtegwqzt.html

openssl rand -hex 16
来源：http://hz.haohaochexian.top/gtmjezgsdy.html

[R68] 计算文件校验值
来源：http://hz.meibo888.top/gtmbxyuajo.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.aibaodan.cn/gtgeyiklgz.html

[R69] 生成随机密码
来源：http://hz.guowangkeji.top/gthomkgwvd.html

head -c 16 /dev/urandom | base64
来源：http://hz.nanxuanxn.top/gtccvjdizi.html

[R70] 时间戳与互转
来源：http://hz.iojbl.cn/gtvrynunbx.html

date +%s;  date -d @1700000000
来源：http://hz.jiagoushi.top/gtqfsgbyev.html

[R71] 日期格式化
来源：http://hz.ehwqpu.com/gtkhhktryl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yonumen.top/gtmnglbreo.html

[R72] 等待端口就绪
来源：http://hz.haohaochexian.top/gtptjwxigr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.feifeiyinyue.top/gtkcaawhuo.html

[R73] 分割大日志
来源：http://hz.andypj.xyz/gtmpllmcpw.html

split -l 1000 big.log part_
来源：http://hz.xylfe.cn/gtxssarflt.html

[R74] 批量重命名
来源：http://hz.chenzaomai.com/gtfehdjtgy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhiwuduotai.top/gtbzbmqwzl.html

[R75] 导出环境变量
来源：http://hz.svipenyu.cn/gtfhvtlmva.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhengqikj.top/gtedjjfvds.html

[R76] 使用临时文件
来源：http://hz.9152youxi.cn/gttmfztakr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtspvkszpp.html

[R77] 读取用户输入
来源：http://hz.daxiang520.top/gtuepgxkdk.html

read -rp "请输入: " ans
来源：http://hz.jinyuanbaomall.cn/gtagtkkrvs.html

[R78] 交互式菜单
来源：http://hz.ehwqpu.com/gtokfdxnju.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.yuanzhike.top/gtehrpdkwp.html

[R79] 解析命令行选项
来源：http://hz.cqqwz.cn/gtpdpnxuac.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.svipenyu.cn/gtylkbgrbk.html

[R80] 查看脚本执行耗时
来源：http://hz.meibo888.top/gtasmzniyo.html

time ./run.sh
来源：http://hz.tanke756.top/gtenllonxe.html

================================================================================
来源：http://hz.ydzc1.top/gtsrrhdlgj.html

S. C / C++ 专题
来源：http://hz.shangyingyoupin.top/gtlybzxvqc.html

================================================================================
来源：http://hz.xinyue.icu/gttigtulxu.html

[S01] C：Hello World
来源：http://hz.shzxlz.cn/gttbpdgyqx.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtjlusrurj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.feifeiyinyue.top/gthxoravzp.html

[S02] C：变量与格式化输出
来源：http://hz.aizwys.cn/gtarezrqcd.html

int a = 10; printf("%d\n", a);
来源：http://hz.hysaishi.cn/gtnrbsrvmw.html

[S03] C：读入整数
来源：http://hz.jlsjyb.cn/gtkimcvnda.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gtceevpaqn.html

[S04] C：字符串复制
来源：http://hz.nanxuanxn.top/gtvyvhhhbf.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gthpduaodu.html

[S05] C：字符串长度
来源：http://hz.yvedp.cn/gtkgamzwkm.html

strlen(s)
来源：http://hz.xylfe.cn/gtuarpyvvd.html

[S06] C：字符串比较
来源：http://hz.yanxiufei.cn/gtjuiyvdlw.html

strcmp(a, b) == 0
来源：http://hz.zhengqikj.top/gtseusbyyr.html

[S07] C：数组遍历求和
来源：http://hz.sxryk.cn/gtvopjdisy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.aibaodan.cn/gtukorzycu.html

[S08] C：动态内存分配与释放
来源：http://hz.cucudq.cn/gthpnrcyqg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.meibo888.top/gtfyyudvkj.html

[S09] C：结构体定义与初始化
来源：http://hz.zhaomingkeji.xyz/gtlxvaovbq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sweek.top/gteqvhxlbq.html

[S10] C：指针与解引用
来源：http://hz.yj202588.top/gtjpbdyqdo.html

int *p = &a;  *p = 5;
来源：http://hz.shanyushiyangkeji.top/gttmqmbyoa.html

[S11] C：逐行读文件
来源：http://hz.ydzc1.top/gtenijmilt.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.jyoumei.cn/gtwwpanbiz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yj20258888.top/gtsjccnfnh.html

fclose(f);
来源：http://hz.xinyue.icu/gtzgngrhmu.html

[S12] C：写文件
来源：http://hz.redwolf501.top/gtsytnelfe.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gzhubu.top/gtstzixxcq.html

[S13] C：宏定义
来源：http://hz.nanxuanxn.top/gtzgsvteif.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.wangshuangyany.cn/gtpbhgghvj.html

[S14] C：枚举
来源：http://hz.hywenlv.cn/gtwreeqhvp.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.9152youxi.cn/gtvipfymhs.html

[S15] C：类型转换
来源：http://hz.xinyue.icu/gtxkceizxj.html

(double) a / b
来源：http://hz.meibo888.top/gtzoruicbu.html

[S16] C：位操作置位
来源：http://hz.chenjidiqi.icu/gtusfiddfd.html

x |= (1 << 3);
来源：http://hz.birdmap.top/gtmpbdbgaf.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtfvwcmvwj.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.jlsjyb.cn/gtoogtaybb.html

[S18] C：命令行参数
来源：http://hz.nanxinkj.top/gtpjektwvi.html

int main(int argc, char **argv)
来源：http://hz.hysaishi.cn/gtqevcaqvj.html

[S19] C：快速排序
来源：http://hz.tian-w.cn/gtaymkfdfo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.vqdsnc.cn/gtjyyepefi.html

[S20] C：二分查找
来源：http://hz.zhengqikj.top/gtnjtxovsk.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ehwqpu.com/gtddcuribm.html

[S21] C：字符类别判断
来源：http://hz.hysaishi.cn/gtqevubyvb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.hfpthk.cn/gteaimbbca.html

[S22] C：字符串转数字
来源：http://hz.0kj1m.cn/gtnoyruayi.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xziqi.cn/gteuilgqks.html

[S23] C：随机数
来源：http://hz.havefunace.top/gtmspxsbgg.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.yuxming.cn/gtazwybffr.html

[S24] C：获取本地时间
来源：http://hz.shangyingyoupin.top/gtnitlqhyt.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.tanke756.top/gtxfqozbea.html

[S25] C：内存拷贝
来源：http://hz.zhaomingkeji.xyz/gtrmbbldtx.html

memcpy(dst, src, n);
来源：http://hz.wangdashe.top/gtneyqfwct.html

[S26] C：内存清零
来源：http://hz.yueranfly.top/gtihgbvgcg.html

memset(a, 0, sizeof a);
来源：http://hz.haohaochexian.top/gtzdyxclld.html

[S27] C：定义常量
来源：http://hz.aizwys.cn/gtiypjsksq.html

const double PI = 3.14159;
来源：http://hz.aibaodan.cn/gthhblbzvq.html

[S28] C：静态变量
来源：http://hz.ivvv.top/gtqsvbhxjs.html

static int counter = 0;
来源：http://hz.0kj1m.cn/gtihgifhvy.html

[S29] C：变参函数
来源：http://hz.redwolf501.top/gtwiusbagy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.xingfuxueyuan.xyz/gtalwtffoc.html

[S30] C：头文件保护
来源：http://hz.cheryme.top/gthhwovtre.html

#ifndef X_H
来源：http://hz.snrcjt.cn/gtjuwxyysk.html

#define X_H
来源：http://hz.xziqi.cn/gtnbhvbokx.html

#endif
来源：http://hz.yuanzhike.top/gtyloyqmja.html

[S31] C++：Hello World
来源：http://hz.chenlongwang.top/gtmkddwllr.html

#include <iostream>
来源：http://hz.shangyingyoupin.top/gtqitdfejd.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.hongshengwenyu.top/gtonhtfmpl.html

[S32] C++：字符串
来源：http://hz.gaohongyu789.top/gtaqctfmys.html

std::string s = "hi";  s += "!";
来源：http://hz.gotoacloud.top/gtmgnkwklf.html

[S33] C++：vector 增删
来源：http://hz.zhengqikj.top/gtouoglouy.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.hfpthk.cn/gtqexydyoo.html

[S34] C++：遍历 vector
来源：http://hz.ydjk.org.cn/gtismeyapp.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.guannengcc.top/gtpbgwhrdz.html

[S35] C++：map
来源：http://hz.cdnleiting.top/gtaaceqpfr.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.yuxming.cn/gtnzfnjdzs.html

[S36] C++：unordered_map
来源：http://hz.redwolf501.top/gtvwhjkgqq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.pycfn.com/gtlllyovgu.html


<!-- 参考信息 -->