代发 wailian999

[Q61] 移动平均
来源：http://hz.zycfv.cn/gtntvwwpfw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhongyouzk.top/gtbtvjhouc.html

[Q62] 分组占比
来源：http://hz.pengpengdd.cyou/gtpexqglud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.tanke756.top/gtlegnnsvz.html

[Q63] 开启事务
来源：http://hz.mhx1999.top/gtzcvnrhio.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.iojbl.cn/gtwmhcfzgg.html

[Q64] 提交事务
来源：http://hz.316326.xyz/gttkyvjwua.html

COMMIT;
来源：http://hz.jlsjyb.cn/gtocvjilvj.html

[Q65] 回滚事务
来源：http://hz.guannengcc.top/gtiangghul.html

ROLLBACK;
来源：http://hz.daria6918.cn/gtemxedvbk.html

[Q66] 行锁查询
来源：http://hz.ydjk.org.cn/gtklruqoty.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.xuanzx.com/gtqdkferio.html

[Q67] 设置隔离级别
来源：http://hz.zhoulong.xyz/gtsbwriclo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.xuanzx.com/gtcguqnann.html

[Q68] 保存点
来源：http://hz.cucudq.cn/gttsicfqei.html

SAVEPOINT sp1;
来源：http://hz.hysaishi.cn/gttbfqtiej.html

ROLLBACK TO sp1;
来源：http://hz.chenjidiqi.icu/gtdzobtfzm.html

[Q69] 查看执行计划
来源：http://hz.tanke756.top/gtdcwqngex.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aibaodan.cn/gteepxubzi.html

[Q70] 更新统计信息
来源：http://hz.smart0.xyz/gtfbxkjqns.html

ANALYZE TABLE users;
来源：http://hz.zhongyouzk.top/gtpejgwqvk.html

[Q71] 查看建表语句
来源：http://hz.cashguo.top/gtugrobkln.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.sufxvd.cn/gtiaczaqsi.html

[Q72] 查看索引
来源：http://hz.gaohongyu789.top/gtotqhroqb.html

SHOW INDEX FROM users;
来源：http://hz.vqdsnc.cn/gtdwkznpus.html

[Q73] 查看表状态
来源：http://hz.yuxming.cn/gtfcfjixen.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sufxvd.cn/gtjizpotqx.html

[Q74] 强制使用索引
来源：http://hz.xylfe.cn/gtgaosjrul.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtriynhkzl.html

[Q75] 日期格式化
来源：http://hz.daria6918.cn/gtnwulsaax.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yonumen.top/gtlrdbbhei.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.xziqi.cn/gtlgyoscbg.html

[Q76] 按天统计
来源：http://hz.316326.xyz/gtdvpkmrxi.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.guannengcc.top/gtjcmsdddi.html

[Q77] 时间加减
来源：http://hz.hywenlv.cn/gteunximyo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.ydjk.org.cn/gtlnrivpko.html

[Q78] 当前时间
来源：http://hz.hammf.cn/gtaxdqfazz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.yuanzhike.top/gtgriqpfpl.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtansxipkb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.shanyushiyangtech.top/gtoezgvpsm.html

[Q80] 字符串截取
来源：http://hz.wangshuangyany.cn/gtaplzcscn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.sxryk.cn/gtqoqfmnjk.html

[Q81] 字符串替换
来源：http://hz.c1oappe.top/gtgoodgmvs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtgfwbffnt.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtesavhpbn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtdcngghtv.html

[Q83] 大小写转换
来源：http://hz.tian-w.cn/gtzjftcrrj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.hongshengwenyu.top/gtcarrhjhk.html

[Q84] 去除首尾空格
来源：http://hz.yongpay.top/gtqfnuvkwu.html

SELECT TRIM(name) FROM users;
来源：http://hz.shzxlz.cn/gttvmltubf.html

[Q85] 数值取整
来源：http://hz.iojbl.cn/gtrnsgjiqk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tian-w.cn/gtifrxgniz.html

[Q86] 读取 JSON 字段
来源：http://hz.zdqjudy.top/gtiqxxmtbk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.andypj.xyz/gtadjtrmau.html

[Q87] JSON 字段做条件
来源：http://hz.zhengqikj.top/gtufvcnyic.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.ydzc1.top/gtxcidikyi.html

[Q88] 行转列（条件聚合）
来源：http://hz.nanxinkj.top/gtpxscxhmg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jinyuanbaomall.cn/gttukhgrzd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yanxiufei.cn/gtmdujvivt.html

[Q89] 判断表是否存在
来源：http://hz.jyoumei.cn/gtrtnwmwyn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.svipenyu.cn/gthqsupahe.html

[Q90] 生成序号列
来源：http://hz.andypj.xyz/gtrjhtwylg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.aizwys.cn/gtgfpzedbd.html

================================================================================
来源：http://hz.pycfn.com/gtxznjrjxh.html

R. Bash 专题
来源：http://hz.dianchejie.cn/gtpgstilrq.html

================================================================================
来源：http://hz.zhijiandao.cn/gtzmyqkpeg.html

[R01] shebang 与严格模式
来源：http://hz.fzhhl.top/gttybnozdm.html

#!/usr/bin/env bash
来源：http://hz.sweek.top/gtxnmaixjy.html

set -euo pipefail
来源：http://hz.ybcxt.top/gtkkvkebbi.html

[R02] 变量赋值与使用
来源：http://hz.shangyingyoupin.top/gtrkuzdelx.html

name="Tom"; echo "$name"
来源：http://hz.jiagoushi.top/gtrhnmpxbe.html

[R03] 只读变量
来源：http://hz.yj20258888.top/gtuvfuvkki.html

readonly PI=3.14
来源：http://hz.hysaishi.cn/gtvcvyctgf.html

[R04] 位置参数
来源：http://hz.zhijiandao.cn/gtrsrqdpvl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.wangshuangyany.cn/gthdmzzlpi.html

[R05] 参数默认值
来源：http://hz.aibaodan.cn/gtxxqrbzsu.html

name="${1:-default}"
来源：http://hz.gaohongyu789.top/gtysltpsju.html

[R06] 判断命令是否存在
来源：http://hz.shanyushiyangkeji.top/gtsiypunao.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.ywan-chungtsiang.top/gtydlwzyxo.html

[R07] if 判断文件
来源：http://hz.shanyushiyangkeji.top/gtuvmexuup.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ppjwa.cn/gtgtyylskp.html

[R08] 数值比较
来源：http://hz.hywenlv.cn/gtptkzzuaj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.iojbl.cn/gtiyewmvzd.html

[R09] 字符串比较
来源：http://hz.yuanzhike.top/gtglarptwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.meibo888.top/gtxdsffrhi.html

[R10] 正则匹配
来源：http://hz.xuanzx.com/gtmborcotu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.hnqzz.top/gtkfemlvuh.html

[R11] case 多分支
来源：http://hz.ivvv.top/gtucoumhdw.html

case "$1" in
来源：http://hz.yj20258.top/gtgwmfkltz.html

start) echo "启动" ;;
来源：http://hz.zycfv.cn/gtymwwvror.html

stop)  echo "停止" ;;
来源：http://hz.jqgufenzy.top/gtexwmkzrl.html

*)     echo "未知命令" ;;
来源：http://hz.chenzaomai.com/gttpxnsnia.html

esac
来源：http://hz.guowangkeji.top/gthovtgalf.html

[R12] for 遍历文件
来源：http://hz.sysykeji.top/gtywpfqnjw.html

for f in *.txt; do echo "$f"; done
来源：http://hz.ywan-chungtsiang.top/gtaaxfiwzn.html

[R13] for 计数循环
来源：http://hz.zhixingplan.top/gtypgipkmp.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.guowangkeji.top/gtbsggsgov.html

[R14] C 风格 for
来源：http://hz.yvedp.cn/gtbznmrxda.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.hnxiangtu.top/gtdgxgvnpk.html

[R15] while 逐行读文件
来源：http://hz.pengpengdd.cyou/gtswbxozny.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ppjwa.cn/gtlhtwfbxw.html

[R16] until 等待条件
来源：http://hz.quarkkingdee.top/gtjfzlidlv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.daxiang520.top/gtozjsnzuu.html

[R17] 数组定义与取值
来源：http://hz.sufxvd.cn/gtrzyxjjda.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtfzfewbis.html

[R18] 遍历数组
来源：http://hz.feifeiyinyue.top/gtharbtypx.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenzaomai.com/gtteqbzdoo.html

[R19] 数组长度
来源：http://hz.xuanzx.com/gtcjckntsa.html

echo "${#arr[@]}"
来源：http://hz.feifeiyinyue.top/gtaovtrcda.html

[R20] 关联数组（字典）
来源：http://hz.chenjidiqi.icu/gthecipzfg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ybcxt.top/gtyfmzneyi.html

[R21] 字符串长度
来源：http://hz.cashguo.top/gtuuccavxg.html

echo "${#s}"
来源：http://hz.shuidangran.top/gtnfckdhni.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtsjhlxhdu.html

echo "${s:0:5}"
来源：http://hz.bjfxy.top/gtvrliqczw.html

[R23] 字符串替换
来源：http://hz.yvedp.cn/gtypaujssz.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.havefunace.top/gtyefgbcjm.html

[R24] 大小写转换
来源：http://hz.xuanzx.com/gtfjbipkeo.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.snrcjt.cn/gtflcjwdrf.html

[R25] 去后缀 / 去前缀
来源：http://hz.pengpengdd.cyou/gtjsviznze.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.meibo888.top/gtmknyfkmq.html

[R26] 命令替换
来源：http://hz.xingfuxueyuan.xyz/gtpzxgsjrw.html

now=$(date +%F); echo "$now"
来源：http://hz.tanke756.top/gtvzretohh.html

[R27] 算术展开
来源：http://hz.jiagoushi.top/gtybeuuowr.html

echo $((1 + 2 * 3))
来源：http://hz.sufxvd.cn/gttzyyhnvw.html

[R28] 浮点运算
来源：http://hz.ydjk.org.cn/gtaqvhgnmf.html

echo "scale=2; 10/3" | bc
来源：http://hz.iojbl.cn/gtvrcyobqp.html

[R29] 定义函数
来源：http://hz.shangyingyoupin.top/gtsrxaxmdu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.jianghu66.top/gtgoqvnjhi.html

[R30] 函数返回状态码
来源：http://hz.aizwys.cn/gtyzpjxqbd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.c1oappe.top/gtenbvnfdd.html

[R31] 局部变量
来源：http://hz.cdnleiting.top/gtuxjmruke.html

f() { local x=1; echo "$x"; }
来源：http://hz.ywan-chungtsiang.top/gtdgfsdnru.html

[R32] 参数个数校验
来源：http://hz.meibo888.top/gtvjmuoida.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yanxiufei.cn/gtvuxuublo.html

[R33] 捕获错误并提示行号
来源：http://hz.cucudq.cn/gtrytpaswy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.daria6918.cn/gttdybzlaq.html

[R34] 退出时清理
来源：http://hz.yongpay.top/gtabysfbzu.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtnojoakwa.html

[R35] 后台执行并等待
来源：http://hz.smart0.xyz/gtqpbznuyw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.pengpengdd.cyou/gtpetziqhc.html

[R36] 并发执行多个任务
来源：http://hz.jqgufenzy.top/gtqewbzhyx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.yvedp.cn/gtmmytaaxv.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtofnlpblm.html

files=$(ls -1)
来源：http://hz.hfpthk.cn/gtbpxzonon.html

[R38] 管道串联
来源：http://hz.hysaishi.cn/gtsrvgtbns.html

cat a.txt | grep -i error | wc -l
来源：http://hz.sxryk.cn/gttsrgxduc.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtleqdqspj.html

cmd > out.log 2>&1
来源：http://hz.iojbl.cn/gteozbfnlh.html

[R40] 追加写日志
来源：http://hz.tanke756.top/gtlxffuyxq.html

echo "log" >> out.log
来源：http://hz.ppjwa.cn/gtvxyyymjb.html

[R41] 丢弃输出
来源：http://hz.wangdashe.top/gtvjkezszp.html

cmd >/dev/null 2>&1
来源：http://hz.zdqjudy.top/gtfhdcnwtm.html

[R42] 输入重定向
来源：http://hz.yj20258888.top/gtzufvmxnl.html

wc -l < a.txt
来源：http://hz.zhaomingkeji.xyz/gtntwnmloy.html

[R43] 按名字查找文件
来源：http://hz.hongshengwenyu.top/gtwujaaeaq.html

find . -name "*.log" -type f
来源：http://hz.zdqjudy.top/gttqvvyugr.html

[R44] 按修改时间查找
来源：http://hz.jinghuilouyu.cn/gtlplpeeaz.html

find . -mtime -7 -type f
来源：http://hz.sufxvd.cn/gtjgqalbtt.html

[R45] 批量删除
来源：http://hz.guowangkeji.top/gtmgabebri.html

find . -name "*.tmp" -delete
来源：http://hz.c1oappe.top/gtvujdfwoe.html

[R46] 递归替换文件内容
来源：http://hz.ivvv.top/gtyhtvmpmn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.jinqigufen.top/gtewkifppw.html

[R47] sed 单行替换
来源：http://hz.tianlin.xyz/gtolmvccpv.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.gaohongyu789.top/gtlgbhrvaf.html

[R48] awk 取指定列
来源：http://hz.tian-w.cn/gtkjeeuume.html

awk '{print $1, $3}' a.txt
来源：http://hz.jlsjyb.cn/gtwwokusbm.html

[R49] awk 带条件
来源：http://hz.sysykeji.top/gticevgqst.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.cucudq.cn/gtajvuqhzl.html

[R50] awk 求和
来源：http://hz.wangshuangyany.cn/gtjetusuyc.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtmnipexbm.html

[R51] 排序去重取前几
来源：http://hz.jyoumei.cn/gtenolzhsn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.cheryme.top/gtryyjlwve.html

[R52] 统计行数
来源：http://hz.xinyue.icu/gtjgtznunk.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtdxsfsasa.html

[R53] 查看文件头与实时尾
来源：http://hz.guowangkeji.top/gtyhqnzcaf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.dianchejie.cn/gtkfnjvbxl.html

[R54] 比较两个文件
来源：http://hz.dashuyun.cn/gtjarufodn.html

diff a.txt b.txt
来源：http://hz.redwolf501.top/gtducgdhec.html

[R55] 压缩与解压
来源：http://hz.haohaochexian.top/gtnlpqejzj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.9152youxi.cn/gteftujcpg.html

[R56] 远程拷贝
来源：http://hz.hnxiangtu.top/gtfzlcltxy.html

scp file user@host:/path/
来源：http://hz.shzxlz.cn/gtmjjieeka.html

[R57] 远程执行命令
来源：http://hz.zhaomingkeji.xyz/gtrkkfandv.html

ssh user@host 'uptime'
来源：http://hz.shanyushiyangtech.top/gtbylfnkuu.html

[R58] 下载文件
来源：http://hz.vqdsnc.cn/gtdovftxft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cdnleiting.top/gtwqvnlwov.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gtxhkdkxss.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.shzxlz.cn/gtwmqwzuxx.html

[R60] 只看 HTTP 状态码
来源：http://hz.xylfe.cn/gthiwjwcuw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sxryk.cn/gttalehmnx.html

[R61] 磁盘占用
来源：http://hz.aibaodan.cn/gtmywnrali.html

df -h;  du -sh *
来源：http://hz.sysykeji.top/gtvqolvkbm.html

[R62] 找最占空间的文件
来源：http://hz.nanxinkj.top/gthpbyhnap.html

du -ah . | sort -rh | head -10
来源：http://hz.nanxuanxn.top/gtowqwtgts.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gtbjgdnrho.html

free -h;  ps aux | grep nginx
来源：http://hz.tianlin.xyz/gtnutjcmob.html

[R64] 结束进程
来源：http://hz.yonumen.top/gtckfnyxrp.html

kill -9 $(pgrep -f app.py)
来源：http://hz.sufxvd.cn/gtykocpjqt.html

[R65] 查看端口占用
来源：http://hz.hysaishi.cn/gtbnnngpnd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.tianlin.xyz/gtodxmszhr.html

[R66] 定时任务
来源：http://hz.iojbl.cn/gtmqtyohbo.html

crontab -e;  crontab -l
来源：http://hz.xziqi.cn/gtvwfulwrx.html

[R67] 生成随机十六进制串
来源：http://hz.c1oappe.top/gtoljjlpdg.html

openssl rand -hex 16
来源：http://hz.yongpay.top/gtxajtenrj.html

[R68] 计算文件校验值
来源：http://hz.0kj1m.cn/gtdzqljjjs.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hysaishi.cn/gtyfwfyyip.html

[R69] 生成随机密码
来源：http://hz.shuidangran.top/gtzxgokual.html

head -c 16 /dev/urandom | base64
来源：http://hz.hammf.cn/gtffdnlgdu.html

[R70] 时间戳与互转
来源：http://hz.wangshuangyany.cn/gtivqmyjbg.html

date +%s;  date -d @1700000000
来源：http://hz.zhongyouzk.top/gtpuopfihy.html

[R71] 日期格式化
来源：http://hz.ydjk.org.cn/gtuffoshsn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.nwbrower.top/gtgfgrednz.html

[R72] 等待端口就绪
来源：http://hz.ydjk.org.cn/gtgmsatfml.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.ydjk.org.cn/gtuewbntuj.html

[R73] 分割大日志
来源：http://hz.hnxiangtu.top/gtupzxosew.html

split -l 1000 big.log part_
来源：http://hz.yueranfly.top/gtwwvcisde.html

[R74] 批量重命名
来源：http://hz.jinghuilouyu.cn/gtzturmhgj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.sxryk.cn/gtzhajqtwa.html

[R75] 导出环境变量
来源：http://hz.zhaomingkeji.xyz/gtysxttoga.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.cheryme.top/gthpdsdabw.html

[R76] 使用临时文件
来源：http://hz.hammf.cn/gtglupsmnj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gthptwdmqs.html

[R77] 读取用户输入
来源：http://hz.sweek.top/gtmruouady.html

read -rp "请输入: " ans
来源：http://hz.shuidangran.top/gtupfppvky.html

[R78] 交互式菜单
来源：http://hz.gzhubu.top/gthlruucqh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.ydzc1.top/gtyhnemwoe.html

[R79] 解析命令行选项
来源：http://hz.pycfn.com/gtvtcyjxtu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.kuanghao11.cn/gtmktazphh.html

[R80] 查看脚本执行耗时
来源：http://hz.gotoacloud.top/gtqnvbbozz.html

time ./run.sh
来源：http://hz.xylfe.cn/gtelbdwnmo.html

================================================================================
来源：http://hz.cashguo.top/gtkmztutlj.html

S. C / C++ 专题
来源：http://hz.xinyue.icu/gtifhdkyak.html

================================================================================
来源：http://hz.zhijiandao.cn/gtjjclexss.html

[S01] C：Hello World
来源：http://hz.tian-w.cn/gtgckqnqae.html

#include <stdio.h>
来源：http://hz.zdqjudy.top/gtptrbosey.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.hfpthk.cn/gtzsuybczk.html

[S02] C：变量与格式化输出
来源：http://hz.kuanghao11.cn/gtyfgfheqe.html

int a = 10; printf("%d\n", a);
来源：http://hz.meibo888.top/gteskkeaal.html

[S03] C：读入整数
来源：http://hz.guannengcc.top/gttprxyawt.html

int x; scanf("%d", &x);
来源：http://hz.vqdsnc.cn/gthycpahoz.html

[S04] C：字符串复制
来源：http://hz.hnqzz.top/gtfuqetioa.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.aizwys.cn/gtpsynpxgc.html

[S05] C：字符串长度
来源：http://hz.yanxiufei.cn/gtierbmgwj.html

strlen(s)
来源：http://hz.jinyuanbaomall.cn/gtodjngfkm.html

[S06] C：字符串比较
来源：http://hz.xinyue.icu/gtrlrbyohb.html

strcmp(a, b) == 0
来源：http://hz.shangyingyoupin.top/gtddfyrdfy.html

[S07] C：数组遍历求和
来源：http://hz.sweek.top/gtxgnssqng.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pengpengdd.cyou/gtiapqwgxx.html

[S08] C：动态内存分配与释放
来源：http://hz.yuanzhike.top/gtufwtrucg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.andypj.xyz/gtegqwhtzn.html

[S09] C：结构体定义与初始化
来源：http://hz.cqqwz.cn/gtwaysufie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.sxryk.cn/gtyozshvug.html

[S10] C：指针与解引用
来源：http://hz.jinyuanbaomall.cn/gtdpclvhzi.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gtkazyiwsf.html

[S11] C：逐行读文件
来源：http://hz.chenlongwang.top/gtppboooek.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.shangyingyoupin.top/gtlsictbna.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.xylfe.cn/gtujwoajat.html

fclose(f);
来源：http://hz.shanyushiyangkeji.top/gtykwrukwc.html

[S12] C：写文件
来源：http://hz.zhaomingkeji.xyz/gtuopqxdxz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.ydzc1.top/gtonpydnqf.html

[S13] C：宏定义
来源：http://hz.gotoacloud.top/gttzobybhh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yanxiufei.cn/gtcspritgs.html

[S14] C：枚举
来源：http://hz.nanxuanxn.top/gtydnizyud.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.havefunace.top/gtjvbutjfu.html

[S15] C：类型转换
来源：http://hz.xuetiantiany.cn/gtanomnrzr.html

(double) a / b
来源：http://hz.birdmap.top/gtncnkgjbw.html

[S16] C：位操作置位
来源：http://hz.nwbrower.top/gtfqhqhcvl.html

x |= (1 << 3);
来源：http://hz.xuetiantiany.cn/gttdpdrgel.html

[S17] C：安全拼接字符串
来源：http://hz.cashguo.top/gtdcqotrau.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenzaomai.com/gtuibdkydd.html

[S18] C：命令行参数
来源：http://hz.jinghuilouyu.cn/gtnhcefnfe.html

int main(int argc, char **argv)
来源：http://hz.hywenlv.cn/gtzdoqxbej.html

[S19] C：快速排序
来源：http://hz.ydzc1.top/gtcknjvquo.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.shangyingyoupin.top/gtdlyhifju.html

[S20] C：二分查找
来源：http://hz.zhiwuduotai.top/gtdkuakaju.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.quarkkingdee.top/gtocpkebgw.html

[S21] C：字符类别判断
来源：http://hz.feifeiyinyue.top/gticwrptiu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.jinyuanbaomall.cn/gtjhydcqwb.html

[S22] C：字符串转数字
来源：http://hz.daria6918.cn/gtxqpddacb.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hnqzz.top/gtxyogtjph.html

[S23] C：随机数
来源：http://hz.gotoacloud.top/gtkdwerpjv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hysaishi.cn/gtntbqyhhv.html

[S24] C：获取本地时间
来源：http://hz.yj20258888.top/gtwuabjnfc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.yongpay.top/gtcawdoizo.html

[S25] C：内存拷贝
来源：http://hz.bjfxy.top/gtilijubns.html

memcpy(dst, src, n);
来源：http://hz.9152youxi.cn/gtbmjsepxs.html

[S26] C：内存清零
来源：http://hz.nwbrower.top/gteoupkizx.html

memset(a, 0, sizeof a);
来源：http://hz.pycfn.com/gttwdtrevl.html

[S27] C：定义常量
来源：http://hz.zhoulong.xyz/gtsvejquyx.html

const double PI = 3.14159;
来源：http://hz.wangshuangyany.cn/gtxmfofrly.html

[S28] C：静态变量
来源：http://hz.ybcxt.top/gtdzyvwkus.html

static int counter = 0;
来源：http://hz.shuidangran.top/gtqykflcvb.html

[S29] C：变参函数
来源：http://hz.ppjwa.cn/gtkhqiqyac.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.ywan-chungtsiang.top/gteeirxfiz.html

[S30] C：头文件保护
来源：http://hz.yvedp.cn/gtnywpkivo.html

#ifndef X_H
来源：http://hz.ybcxt.top/gtttspqjye.html

#define X_H
来源：http://hz.nanxinkj.top/gtuydfgsmo.html

#endif
来源：http://hz.svipenyu.cn/gtmliexyhj.html

[S31] C++：Hello World
来源：http://hz.gaohongyu789.top/gtjckjxdjk.html


<!-- 参考信息 -->