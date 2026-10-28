代发 wailian999

[Q67] 设置隔离级别
来源：http://hz.ydjk.org.cn/gtharpnhfb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yangfankeji.com/gtbbdgktlx.html

[Q68] 保存点
来源：http://hz.yvedp.cn/gtfdvysdcu.html

SAVEPOINT sp1;
来源：http://hz.gotoacloud.top/gtideyhcbq.html

ROLLBACK TO sp1;
来源：http://hz.chenzaomai.com/gtetbraydb.html

[Q69] 查看执行计划
来源：http://hz.hywenlv.cn/gtuoaxakke.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hfpthk.cn/gtrnqnpzvd.html

[Q70] 更新统计信息
来源：http://hz.redwolf501.top/gtmzpphunl.html

ANALYZE TABLE users;
来源：http://hz.sysykeji.top/gtmhjuduct.html

[Q71] 查看建表语句
来源：http://hz.zhijiandao.cn/gtckomjiql.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.jinqigfzy.top/gtryrkeqat.html

[Q72] 查看索引
来源：http://hz.hammf.cn/gtiqnbtmwg.html

SHOW INDEX FROM users;
来源：http://hz.wangshuangyany.cn/gtapofdaiq.html

[Q73] 查看表状态
来源：http://hz.yuanzhike.top/gtsrdxalkn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.c1oappe.top/gtvyacbwof.html

[Q74] 强制使用索引
来源：http://hz.yvedp.cn/gtgtwzqwrn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.cdnleiting.top/gtuepjveab.html

[Q75] 日期格式化
来源：http://hz.yvedp.cn/gtoygrynvd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.hysaishi.cn/gtoiqcqvrv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yj20258888.top/gtmohxnsrf.html

[Q76] 按天统计
来源：http://hz.jqgufenzy.top/gtgclrsbzm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.sufxvd.cn/gtpdzbfxck.html

[Q77] 时间加减
来源：http://hz.ydzc1.top/gtyetirbff.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtunswstbq.html

[Q78] 当前时间
来源：http://hz.jlsjyb.cn/gtcarbcsze.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.guowangkeji.top/gtjokntsgd.html

[Q79] 字符串拼接
来源：http://hz.jinqigufen.top/gtbzxrluzi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.zhixingplan.top/gtdepqnniv.html

[Q80] 字符串截取
来源：http://hz.jiagoushi.top/gtpdavnboz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangdashe.top/gtegrxnzhn.html

[Q81] 字符串替换
来源：http://hz.zhoulong.xyz/gtmsmikguy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.birdmap.top/gtpfzobmav.html

[Q82] 字符长度与字节长度
来源：http://hz.hnqzz.top/gtppqgueax.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yj20258.top/gtjxiigbhq.html

[Q83] 大小写转换
来源：http://hz.aizwys.cn/gtpxdcpkib.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.yangfankeji.com/gtrhodifdo.html

[Q84] 去除首尾空格
来源：http://hz.zhaomingkeji.xyz/gtfoesfjef.html

SELECT TRIM(name) FROM users;
来源：http://hz.jinghuilouyu.cn/gtcbwnxebp.html

[Q85] 数值取整
来源：http://hz.0kj1m.cn/gthiuqbjmu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.daria6918.cn/gtwtknhfhq.html

[Q86] 读取 JSON 字段
来源：http://hz.guannengcc.top/gtahpxqkxy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gtopabmymq.html

[Q87] JSON 字段做条件
来源：http://hz.xylfe.cn/gtathivcod.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.zycfv.cn/gtfhglvobz.html

[Q88] 行转列（条件聚合）
来源：http://hz.gaohongyu789.top/gtdbiancxa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.meibo888.top/gtnzxpannw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.zhaomingkeji.xyz/gthdenfonk.html

[Q89] 判断表是否存在
来源：http://hz.wangshuangyany.cn/gtqpkyutzj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.cashguo.top/gtspoyyzer.html

[Q90] 生成序号列
来源：http://hz.xylfe.cn/gtwxgvjhbu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.xuanzx.com/gtuywwhnvp.html

================================================================================
来源：http://hz.pycfn.com/gtzgadnrxb.html

R. Bash 专题
来源：http://hz.guannengcc.top/gtdrjoyxvh.html

================================================================================
来源：http://hz.ydzc1.top/gtuhkbcpje.html

[R01] shebang 与严格模式
来源：http://hz.xingfuxueyuan.xyz/gtvpxrnvbe.html

#!/usr/bin/env bash
来源：http://hz.hnxiangtu.top/gtihxidtkb.html

set -euo pipefail
来源：http://hz.yj20258888.top/gtbiirgvli.html

[R02] 变量赋值与使用
来源：http://hz.cqqwz.cn/gtffuxssuu.html

name="Tom"; echo "$name"
来源：http://hz.hfpthk.cn/gtpouvbyhn.html

[R03] 只读变量
来源：http://hz.cheryme.top/gtodsdhjni.html

readonly PI=3.14
来源：http://hz.smart0.xyz/gtpmrhojbj.html

[R04] 位置参数
来源：http://hz.sysykeji.top/gtcmafjthf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jianghu66.top/gtepvurntp.html

[R05] 参数默认值
来源：http://hz.meibo888.top/gtajwbkvfq.html

name="${1:-default}"
来源：http://hz.sufxvd.cn/gtmqyejxqa.html

[R06] 判断命令是否存在
来源：http://hz.9152youxi.cn/gtgjywzihg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.guowangkeji.top/gtcjpgstjn.html

[R07] if 判断文件
来源：http://hz.xuetiantiany.cn/gtltilcyuz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtqycmxqcg.html

[R08] 数值比较
来源：http://hz.zhiwuduotai.top/gtxzzwoqdv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtzfxuieor.html

[R09] 字符串比较
来源：http://hz.wangshuangyany.cn/gtdmbfqzno.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.jlsjyb.cn/gtdwhixzbf.html

[R10] 正则匹配
来源：http://hz.yongpay.top/gtttshqbds.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.shuidangran.top/gtrqrvdtqd.html

[R11] case 多分支
来源：http://hz.feifeiyinyue.top/gtxjcsbemc.html

case "$1" in
来源：http://hz.kuanghao11.cn/gtcufkktqb.html

start) echo "启动" ;;
来源：http://hz.svipenyu.cn/gtnzdgtxqn.html

stop)  echo "停止" ;;
来源：http://hz.zhaomingkeji.xyz/gtrjmmbfep.html

*)     echo "未知命令" ;;
来源：http://hz.jinqigufen.top/gtjktrhhpp.html

esac
来源：http://hz.yj20258.top/gtfphehvnr.html

[R12] for 遍历文件
来源：http://hz.tian-w.cn/gtahqkvdtd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.bjfxy.top/gtfvfzyzmi.html

[R13] for 计数循环
来源：http://hz.hnqzz.top/gtfboqvutj.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtrewrysrd.html

[R14] C 风格 for
来源：http://hz.9152youxi.cn/gtnogqlost.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.aibaodan.cn/gtjsdvymoy.html

[R15] while 逐行读文件
来源：http://hz.cqqwz.cn/gtzidvzjox.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtqnoyqpri.html

[R16] until 等待条件
来源：http://hz.dashuyun.cn/gtgocjsxxe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sweek.top/gtgohnzryu.html

[R17] 数组定义与取值
来源：http://hz.hammf.cn/gtcixkqxca.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.9152youxi.cn/gtpexdzlsc.html

[R18] 遍历数组
来源：http://hz.gotoacloud.top/gtnjxrhavt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.quarkkingdee.top/gttmvathsh.html

[R19] 数组长度
来源：http://hz.hfpthk.cn/gtimojvfot.html

echo "${#arr[@]}"
来源：http://hz.mhx1999.top/gttwkszhyi.html

[R20] 关联数组（字典）
来源：http://hz.yonumen.top/gtedfevmub.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.fzhhl.top/gtyhvqmbvi.html

[R21] 字符串长度
来源：http://hz.shanyushiyangkeji.top/gtpctpvzcw.html

echo "${#s}"
来源：http://hz.quarkkingdee.top/gtquenrkpm.html

[R22] 截取子串
来源：http://hz.jqgfzy.top/gtovbqdkts.html

echo "${s:0:5}"
来源：http://hz.sufxvd.cn/gtgclrwtpb.html

[R23] 字符串替换
来源：http://hz.jinqigfzy.top/gtgeiagqub.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.0kj1m.cn/gtxfluqutf.html

[R24] 大小写转换
来源：http://hz.tanke756.top/gtbcjmjvkk.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuanzx.com/gtvqsbudrz.html

[R25] 去后缀 / 去前缀
来源：http://hz.zhixingplan.top/gtfeqbakwh.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.yj20258.top/gtwokfwurl.html

[R26] 命令替换
来源：http://hz.ywan-chungtsiang.top/gttmgzcxlq.html

now=$(date +%F); echo "$now"
来源：http://hz.iojbl.cn/gthnyelhmr.html

[R27] 算术展开
来源：http://hz.316326.xyz/gtwtlndmyz.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gtinjikogy.html

[R28] 浮点运算
来源：http://hz.havefunace.top/gtegfnpftt.html

echo "scale=2; 10/3" | bc
来源：http://hz.quarkkingdee.top/gtgqweaufj.html

[R29] 定义函数
来源：http://hz.yvedp.cn/gtfvbrokix.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jinyuanbaomall.cn/gtmsrnmwjm.html

[R30] 函数返回状态码
来源：http://hz.shanyushiyangkeji.top/gtebosipfw.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.vqdsnc.cn/gtcqhfrfzx.html

[R31] 局部变量
来源：http://hz.hongshengwenyu.top/gtioishgqv.html

f() { local x=1; echo "$x"; }
来源：http://hz.yj20258888.top/gteivqnfyj.html

[R32] 参数个数校验
来源：http://hz.vqdsnc.cn/gtzmkqzriu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenzaomai.com/gtzdfypozj.html

[R33] 捕获错误并提示行号
来源：http://hz.dianchejie.cn/gthwqetzvm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.dashuyun.cn/gtynkayaqv.html

[R34] 退出时清理
来源：http://hz.nanxuanxn.top/gtotkpyzup.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.quarkkingdee.top/gtyfgmyqdv.html

[R35] 后台执行并等待
来源：http://hz.jinghuilouyu.cn/gtfkpispgq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pengpengdd.cyou/gtwjvcazio.html

[R36] 并发执行多个任务
来源：http://hz.bjfxy.top/gtcorlmsli.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ehwqpu.com/gtaufkchpv.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gtnemfqchc.html

files=$(ls -1)
来源：http://hz.yueranfly.top/gtyniwxpjf.html

[R38] 管道串联
来源：http://hz.cucudq.cn/gtlyizznvt.html

cat a.txt | grep -i error | wc -l
来源：http://hz.yj20258.top/gtzqopkkeu.html

[R39] 重定向标准输出与错误
来源：http://hz.nanxuanxn.top/gtwpfyvwdl.html

cmd > out.log 2>&1
来源：http://hz.gotoacloud.top/gtehlugnkj.html

[R40] 追加写日志
来源：http://hz.snrcjt.cn/gtqxfvqaaj.html

echo "log" >> out.log
来源：http://hz.haohaochexian.top/gtxkoydxzs.html

[R41] 丢弃输出
来源：http://hz.ywan-chungtsiang.top/gtkiyezcpz.html

cmd >/dev/null 2>&1
来源：http://hz.yj20258888.top/gtfvxrnswv.html

[R42] 输入重定向
来源：http://hz.jinqigfzy.top/gtpkmblowk.html

wc -l < a.txt
来源：http://hz.andypj.xyz/gtnlneflpv.html

[R43] 按名字查找文件
来源：http://hz.shangyingyoupin.top/gtjmgtqdlv.html

find . -name "*.log" -type f
来源：http://hz.zhengqikj.top/gtalaesznb.html

[R44] 按修改时间查找
来源：http://hz.aibaodan.cn/gtmdiqzinl.html

find . -mtime -7 -type f
来源：http://hz.yj20258888.top/gtcuaoxehe.html

[R45] 批量删除
来源：http://hz.shanyushiyangkeji.top/gtlfyvceuw.html

find . -name "*.tmp" -delete
来源：http://hz.zycfv.cn/gtdagrbigw.html

[R46] 递归替换文件内容
来源：http://hz.chenjidiqi.icu/gtpxbtlxir.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.52xcode.cn/gtbffwhkvy.html

[R47] sed 单行替换
来源：http://hz.haohaochexian.top/gtnftsaszd.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yangfankeji.com/gtxisrgvhf.html

[R48] awk 取指定列
来源：http://hz.chenzaomai.com/gtoxdoragn.html

awk '{print $1, $3}' a.txt
来源：http://hz.aizwys.cn/gtdqzjvcvk.html

[R49] awk 带条件
来源：http://hz.daxiang520.top/gtqgktlwaj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xylfe.cn/gtdinedjsl.html

[R50] awk 求和
来源：http://hz.yj20258888.top/gtntibawus.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jyoumei.cn/gtljyvokan.html

[R51] 排序去重取前几
来源：http://hz.dashuyun.cn/gtcexttmzp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.c1oappe.top/gtpwzcvcnx.html

[R52] 统计行数
来源：http://hz.cheryme.top/gtbksebjju.html

wc -l a.txt
来源：http://hz.jinghuilouyu.cn/gtwhgebigy.html

[R53] 查看文件头与实时尾
来源：http://hz.ywan-chungtsiang.top/gtpzpjwnqf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.aizwys.cn/gtumrecdmu.html

[R54] 比较两个文件
来源：http://hz.chenzaomai.com/gtieclxszb.html

diff a.txt b.txt
来源：http://hz.zhixingplan.top/gtiiuttbqg.html

[R55] 压缩与解压
来源：http://hz.fzhhl.top/gtixgnavfi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gtlqgoysfw.html

[R56] 远程拷贝
来源：http://hz.hammf.cn/gtuqkwxzmd.html

scp file user@host:/path/
来源：http://hz.dianchejie.cn/gthdvsnwpu.html

[R57] 远程执行命令
来源：http://hz.yangfankeji.com/gtxwmtmebr.html

ssh user@host 'uptime'
来源：http://hz.zdqjudy.top/gtgnmxsunw.html

[R58] 下载文件
来源：http://hz.shuidangran.top/gtvilxjftu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.c1oappe.top/gtobfonaky.html

[R59] 发 POST JSON
来源：http://hz.vqdsnc.cn/gtqsdseclg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shanyushiyangkeji.top/gtihddcbxx.html

[R60] 只看 HTTP 状态码
来源：http://hz.wangdashe.top/gtsdqfrupj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yanxiufei.cn/gtcvemsjdg.html

[R61] 磁盘占用
来源：http://hz.jlsjyb.cn/gtrqlucjas.html

df -h;  du -sh *
来源：http://hz.yangfankeji.com/gtcpfftqmh.html

[R62] 找最占空间的文件
来源：http://hz.hysaishi.cn/gtllcxpxwp.html

du -ah . | sort -rh | head -10
来源：http://hz.sweek.top/gthhsprlxh.html

[R63] 内存与进程
来源：http://hz.ybcxt.top/gtvrdjumvy.html

free -h;  ps aux | grep nginx
来源：http://hz.cdnleiting.top/gtbxjjvkca.html

[R64] 结束进程
来源：http://hz.hammf.cn/gtglxkxwpl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.ybcxt.top/gtzusquetk.html

[R65] 查看端口占用
来源：http://hz.fzhhl.top/gtpajwkheh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.fengsongda.top/gttlfitfwx.html

[R66] 定时任务
来源：http://hz.zhijiandao.cn/gtxzlsvtax.html

crontab -e;  crontab -l
来源：http://hz.jiagoushi.top/gtcmnkeiqc.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gtxmueihmp.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtydiwwwlh.html

[R68] 计算文件校验值
来源：http://hz.shanyushiyangkeji.top/gtycouxosx.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhengqikj.top/gtclfsptdr.html

[R69] 生成随机密码
来源：http://hz.zdqjudy.top/gtrfsmzmwu.html

head -c 16 /dev/urandom | base64
来源：http://hz.gaohongyu789.top/gtlabyauzm.html

[R70] 时间戳与互转
来源：http://hz.hnqzz.top/gtdagmxzpj.html

date +%s;  date -d @1700000000
来源：http://hz.gotoacloud.top/gtgsvhippr.html

[R71] 日期格式化
来源：http://hz.zhengqikj.top/gtabdzafdt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.snrcjt.cn/gtenjohlhs.html

[R72] 等待端口就绪
来源：http://hz.zhiwuduotai.top/gthpopcwvi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtnffbrzmr.html

[R73] 分割大日志
来源：http://hz.chenzaomai.com/gtvcnwdovq.html

split -l 1000 big.log part_
来源：http://hz.9152youxi.cn/gthejouibx.html

[R74] 批量重命名
来源：http://hz.sweek.top/gtnnnyiczr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zhijiandao.cn/gtwsffsuch.html

[R75] 导出环境变量
来源：http://hz.yj20258.top/gtqudwtknk.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.gzhubu.top/gtrywmpyon.html

[R76] 使用临时文件
来源：http://hz.yj202588.top/gtevkkwdmt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yj202588.top/gtepcphutc.html

[R77] 读取用户输入
来源：http://hz.nwbrower.top/gtyayvojro.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtfjurntjt.html

[R78] 交互式菜单
来源：http://hz.hnqzz.top/gtqvsruaot.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnxiangtu.top/gtqhnneswq.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtzdshtfpu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.quarkkingdee.top/gtckmqolzk.html

[R80] 查看脚本执行耗时
来源：http://hz.sweek.top/gtemtowext.html

time ./run.sh
来源：http://hz.gaohongyu789.top/gtfodycgul.html

================================================================================
来源：http://hz.ppjwa.cn/gtnifljpog.html

S. C / C++ 专题
来源：http://hz.shangyingyoupin.top/gtvyyixerb.html

================================================================================
来源：http://hz.sweek.top/gtutquamvf.html

[S01] C：Hello World
来源：http://hz.chenjidiqi.icu/gtzspovhrx.html

#include <stdio.h>
来源：http://hz.iojbl.cn/gtpsogqbbv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.jinqigufen.top/gtlpqxcdfu.html

[S02] C：变量与格式化输出
来源：http://hz.tian-w.cn/gtqexfusmd.html

int a = 10; printf("%d\n", a);
来源：http://hz.daxiang520.top/gtekrvxood.html

[S03] C：读入整数
来源：http://hz.c1oappe.top/gtyjbkmnie.html

int x; scanf("%d", &x);
来源：http://hz.yonumen.top/gtsjjickuk.html

[S04] C：字符串复制
来源：http://hz.xuanzx.com/gtjcyiqiwi.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.ywan-chungtsiang.top/gtyglpxcoq.html

[S05] C：字符串长度
来源：http://hz.cheryme.top/gtgriactzn.html

strlen(s)
来源：http://hz.xingfuxueyuan.xyz/gtgituaugm.html

[S06] C：字符串比较
来源：http://hz.svipenyu.cn/gtjhrijhyn.html

strcmp(a, b) == 0
来源：http://hz.havefunace.top/gterhuthbc.html

[S07] C：数组遍历求和
来源：http://hz.fengsongda.top/gtoutazdmi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.0kj1m.cn/gtefvcshvt.html

[S08] C：动态内存分配与释放
来源：http://hz.gzhubu.top/gtzvoamrkx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yuxming.cn/gtofjuqwej.html

[S09] C：结构体定义与初始化
来源：http://hz.jianghu66.top/gtihphtfod.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ydzc1.top/gtgfamhddi.html

[S10] C：指针与解引用
来源：http://hz.pycfn.com/gtcwpasuzo.html

int *p = &a;  *p = 5;
来源：http://hz.redwolf501.top/gtgiezvohk.html

[S11] C：逐行读文件
来源：http://hz.meibo888.top/gtbnybrwwi.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.yanxiufei.cn/gtqxgjiccx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.zhoulong.xyz/gtuhepzonl.html

fclose(f);
来源：http://hz.vqdsnc.cn/gtoiovrgqq.html

[S12] C：写文件
来源：http://hz.sweek.top/gtebyovsee.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.hammf.cn/gtivyblhqa.html

[S13] C：宏定义
来源：http://hz.ivvv.top/gtkqmodqpi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.nanxinkj.top/gtsjtcdbnr.html

[S14] C：枚举
来源：http://hz.c1oappe.top/gtidkwebsj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.sweek.top/gttbhsijwf.html

[S15] C：类型转换
来源：http://hz.yangfankeji.com/gtugkuepdi.html

(double) a / b
来源：http://hz.iojbl.cn/gtdaijaayw.html

[S16] C：位操作置位
来源：http://hz.gotoacloud.top/gtfkhknbxo.html

x |= (1 << 3);
来源：http://hz.jinghuilouyu.cn/gtcvglonsu.html

[S17] C：安全拼接字符串
来源：http://hz.smart0.xyz/gttizgidjc.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.snrcjt.cn/gtsltxzyoj.html

[S18] C：命令行参数
来源：http://hz.smart0.xyz/gtwoejbcuc.html

int main(int argc, char **argv)
来源：http://hz.hfpthk.cn/gtmyashnqz.html

[S19] C：快速排序
来源：http://hz.smart0.xyz/gtjikqaaic.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtpaunlijp.html

[S20] C：二分查找
来源：http://hz.tian-w.cn/gtewmwdkpi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.hywenlv.cn/gtlxdymhwe.html

[S21] C：字符类别判断
来源：http://hz.dashuyun.cn/gtpzngzdrp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yuanzhike.top/gtmoilfjds.html

[S22] C：字符串转数字
来源：http://hz.cheryme.top/gtitaagglu.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.feifeiyinyue.top/gtjpebbeaf.html

[S23] C：随机数
来源：http://hz.ybcxt.top/gtzxojkaox.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.sufxvd.cn/gtcsjtsxaw.html

[S24] C：获取本地时间
来源：http://hz.jqgufenzy.top/gtkxrnuilw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.guowangkeji.top/gtbftqacpl.html

[S25] C：内存拷贝
来源：http://hz.pengpengdd.cyou/gtqivsmccp.html

memcpy(dst, src, n);
来源：http://hz.c1oappe.top/gtcpxknwbc.html

[S26] C：内存清零
来源：http://hz.jyoumei.cn/gthsocgjyl.html

memset(a, 0, sizeof a);
来源：http://hz.birdmap.top/gtrubixdxa.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gtjfqavqyx.html

const double PI = 3.14159;
来源：http://hz.sweek.top/gtyvqidkzv.html

[S28] C：静态变量
来源：http://hz.0kj1m.cn/gtfsyjaeup.html

static int counter = 0;
来源：http://hz.chenjidiqi.icu/gtzynilfhk.html

[S29] C：变参函数
来源：http://hz.iojbl.cn/gtplemhvcb.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.shanyushiyangtech.top/gtlzlmwbue.html

[S30] C：头文件保护
来源：http://hz.zhixingplan.top/gtxqduxlye.html

#ifndef X_H
来源：http://hz.xinyue.icu/gtfpsijhqf.html

#define X_H
来源：http://hz.ppjwa.cn/gtlngyrfoe.html

#endif
来源：http://hz.yangfankeji.com/gtbsspovlv.html

[S31] C++：Hello World
来源：http://hz.andypj.xyz/gtuleyntjv.html

#include <iostream>
来源：http://hz.fzhhl.top/gtmamtsmre.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.dianchejie.cn/gtrmzoybke.html

[S32] C++：字符串
来源：http://hz.yueranfly.top/gtnupnlhil.html

std::string s = "hi";  s += "!";
来源：http://hz.zhengqikj.top/gtobyqjljh.html

[S33] C++：vector 增删
来源：http://hz.snrcjt.cn/gtehglmtpp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hz.shuidangran.top/gtqqcauhnt.html

[S34] C++：遍历 vector
来源：http://hz.zhiwuduotai.top/gtagzwrkbg.html

for (auto &x : v) { std::cout << x; }
来源：http://hz.ehwqpu.com/gtvlmmwhkx.html

[S35] C++：map
来源：http://hz.aizwys.cn/gtzshopgdl.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hz.xziqi.cn/gtktqhrgyj.html

[S36] C++：unordered_map
来源：http://hz.dianchejie.cn/gtsbaiqojx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hz.ppjwa.cn/gttozowpez.html


<!-- 参考信息 -->