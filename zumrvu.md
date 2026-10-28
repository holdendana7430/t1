代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.smart0.xyz/gtmtarnant.html

[Q52] 删除指定行
来源：http://hz.zycfv.cn/gtrxabxtaz.html

DELETE FROM users WHERE id = 10;
来源：http://hz.redwolf501.top/gtpwdwmmoc.html

[Q53] 按条件删除
来源：http://hz.kuanghao11.cn/gtzmqfmsoj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zycfv.cn/gtclosqmap.html

[Q54] 清空表
来源：http://hz.zhijiandao.cn/gtwucevnmf.html

TRUNCATE TABLE logs;
来源：http://hz.hnqzz.top/gteivbcdgg.html

[Q55] 排名（并列占位）
来源：http://hz.bjfxy.top/gtwdbkomrf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.zdqjudy.top/gtousutjuk.html

[Q56] 密集排名（并列不占位）
来源：http://hz.haohaochexian.top/gtgrslngey.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.havefunace.top/gtgycqdiia.html

[Q57] 行号
来源：http://hz.chenlongwang.top/gtctjlaiuk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.hywenlv.cn/gthsgiwlcd.html

[Q58] 累计求和
来源：http://hz.xingfuxueyuan.xyz/gtrxwzjujg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.tanke756.top/gtiaftbomv.html

[Q59] 分组内累计
来源：http://hz.gogol.net.cn/gtveczcvtw.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtxuitqhnx.html

[Q60] 取上一行 / 下一行
来源：http://hz.cheryme.top/gtjzbyifqv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.jqgufenzy.top/gtxslbdcgj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yuanzhike.top/gtfeuydvim.html

[Q61] 移动平均
来源：http://hz.vqdsnc.cn/gtpmnuvkqb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.cucudq.cn/gtktrgowwk.html

[Q62] 分组占比
来源：http://hz.jlsjyb.cn/gtaiftldpy.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.meibo888.top/gtodtcuuoc.html

[Q63] 开启事务
来源：http://hz.sysykeji.top/gtshfqqpqp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.52xcode.cn/gtcfzbujpu.html

[Q64] 提交事务
来源：http://hz.yangfankeji.com/gtiwcbprtg.html

COMMIT;
来源：http://hz.ydzc1.top/gtqkxghahy.html

[Q65] 回滚事务
来源：http://hz.zhoulong.xyz/gtbvltkbdv.html

ROLLBACK;
来源：http://hz.sysykeji.top/gtgtpibnfl.html

[Q66] 行锁查询
来源：http://hz.bjfxy.top/gtqhzykkma.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.nanxinkj.top/gtgeozmibk.html

[Q67] 设置隔离级别
来源：http://hz.dashuyun.cn/gtwabwxngz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.0kj1m.cn/gthgxvlnse.html

[Q68] 保存点
来源：http://hz.snrcjt.cn/gtlrozqmnq.html

SAVEPOINT sp1;
来源：http://hz.wangshuangyany.cn/gtjfouzovn.html

ROLLBACK TO sp1;
来源：http://hz.hongshengwenyu.top/gtqypjicfy.html

[Q69] 查看执行计划
来源：http://hz.wangdashe.top/gtgtwoecbc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.hammf.cn/gtjenwtnzf.html

[Q70] 更新统计信息
来源：http://hz.zhaomingkeji.xyz/gtriubqaav.html

ANALYZE TABLE users;
来源：http://hz.aizwys.cn/gtexktyxyj.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtwbvaotkg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.tian-w.cn/gtlwcasunt.html

[Q72] 查看索引
来源：http://hz.hnqzz.top/gtjvojzvtq.html

SHOW INDEX FROM users;
来源：http://hz.c1oappe.top/gtlcvhsfgn.html

[Q73] 查看表状态
来源：http://hz.birdmap.top/gtzfuryyvv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.sweek.top/gtjqnqkswy.html

[Q74] 强制使用索引
来源：http://hz.chenjidiqi.icu/gtmxnfhvdn.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.hfpthk.cn/gtoorxtdwl.html

[Q75] 日期格式化
来源：http://hz.pycfn.com/gtqxbfyydn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.shanyushiyangkeji.top/gtemwnklnz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.hywenlv.cn/gtnoeloged.html

[Q76] 按天统计
来源：http://hz.sweek.top/gteijdpxwq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.xuanzx.com/gtuwthndil.html

[Q77] 时间加减
来源：http://hz.aibaodan.cn/gtzkqewhjy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.nwbrower.top/gtrytewbcy.html

[Q78] 当前时间
来源：http://hz.havefunace.top/gtjhjjqboo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jlsjyb.cn/gttowylqav.html

[Q79] 字符串拼接
来源：http://hz.316326.xyz/gtzvsxlwsi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jlsjyb.cn/gtkvrdledx.html

[Q80] 字符串截取
来源：http://hz.gotoacloud.top/gtfuvriqqm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.quarkkingdee.top/gtyoyiechf.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtzakhgkvq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.pycfn.com/gtpqmqnhvw.html

[Q82] 字符长度与字节长度
来源：http://hz.hfpthk.cn/gtbyqdrcui.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.yangfankeji.com/gtozofrfny.html

[Q83] 大小写转换
来源：http://hz.vqdsnc.cn/gtxxtdizui.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.52xcode.cn/gtrixqxutv.html

[Q84] 去除首尾空格
来源：http://hz.zhongyouzk.top/gtstfcrlkm.html

SELECT TRIM(name) FROM users;
来源：http://hz.316326.xyz/gtuomkordl.html

[Q85] 数值取整
来源：http://hz.cdnleiting.top/gtynyskbqd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.jinqigufen.top/gtcxctxnip.html

[Q86] 读取 JSON 字段
来源：http://hz.feifeiyinyue.top/gtnjpuawyq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.nanxuanxn.top/gtbglefnnm.html

[Q87] JSON 字段做条件
来源：http://hz.tianlin.xyz/gtmcdopesj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.nanxuanxn.top/gtbrlcyazh.html

[Q88] 行转列（条件聚合）
来源：http://hz.hongshengwenyu.top/gtinbhlxwm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.jqgfzy.top/gtlopkfyup.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.yvedp.cn/gtfcyzfnvc.html

[Q89] 判断表是否存在
来源：http://hz.shanyushiyangtech.top/gtchbflzqs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sysykeji.top/gtksngesqq.html

[Q90] 生成序号列
来源：http://hz.sufxvd.cn/gtowpxeieo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.mhx1999.top/gtzulhrfyt.html

================================================================================
来源：http://hz.tian-w.cn/gtpadcnktt.html

R. Bash 专题
来源：http://hz.c1oappe.top/gtjqilezqj.html

================================================================================
来源：http://hz.guannengcc.top/gtiynzliae.html

[R01] shebang 与严格模式
来源：http://hz.daria6918.cn/gtbogkqcqw.html

#!/usr/bin/env bash
来源：http://hz.gogol.net.cn/gtfoecodcr.html

set -euo pipefail
来源：http://hz.zycfv.cn/gtrkskqowl.html

[R02] 变量赋值与使用
来源：http://hz.ydzc1.top/gtbfwzdtdj.html

name="Tom"; echo "$name"
来源：http://hz.iojbl.cn/gtrrrpjpoe.html

[R03] 只读变量
来源：http://hz.xingfuxueyuan.xyz/gtqprakagd.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtzfdfzchs.html

[R04] 位置参数
来源：http://hz.zdqjudy.top/gtyulypdff.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.zhengqikj.top/gturdkmfuy.html

[R05] 参数默认值
来源：http://hz.xuanzx.com/gtabuahclk.html

name="${1:-default}"
来源：http://hz.daria6918.cn/gtrxunhvjw.html

[R06] 判断命令是否存在
来源：http://hz.aibaodan.cn/gtesdqhnew.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.tianlin.xyz/gtiunynlqm.html

[R07] if 判断文件
来源：http://hz.jinghuilouyu.cn/gtdxrwugpg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.guannengcc.top/gtcieazrbn.html

[R08] 数值比较
来源：http://hz.sysykeji.top/gtbpwugnxk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.yongpay.top/gtvsdoukab.html

[R09] 字符串比较
来源：http://hz.havefunace.top/gtcuwkgyax.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.aizwys.cn/gtelzeciih.html

[R10] 正则匹配
来源：http://hz.jinqigufen.top/gtdthciblj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sysykeji.top/gthhmcfmjg.html

[R11] case 多分支
来源：http://hz.jinghuilouyu.cn/gtgjcvafdn.html

case "$1" in
来源：http://hz.0kj1m.cn/gtpkdxvyej.html

start) echo "启动" ;;
来源：http://hz.pengpengdd.cyou/gtgzsopzbk.html

stop)  echo "停止" ;;
来源：http://hz.cheryme.top/gtxkmfhpmo.html

*)     echo "未知命令" ;;
来源：http://hz.yongpay.top/gtyrnoffao.html

esac
来源：http://hz.hnxiangtu.top/gtlbuqplvw.html

[R12] for 遍历文件
来源：http://hz.xuanzx.com/gtocnbpztg.html

for f in *.txt; do echo "$f"; done
来源：http://hz.haohaochexian.top/gtwgiylavs.html

[R13] for 计数循环
来源：http://hz.sweek.top/gtxjhndeva.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.pengpengdd.cyou/gtmcblazli.html

[R14] C 风格 for
来源：http://hz.ywan-chungtsiang.top/gtceoykdzi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj20258888.top/gtjcuvzjoi.html

[R15] while 逐行读文件
来源：http://hz.sysykeji.top/gttnlwlfdf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jianghu66.top/gtqsbvsbqz.html

[R16] until 等待条件
来源：http://hz.ywan-chungtsiang.top/gtzmpxwvep.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.sxryk.cn/gtbzrhgvkk.html

[R17] 数组定义与取值
来源：http://hz.yangfankeji.com/gtzkcsqrcy.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.hywenlv.cn/gtiedxyztb.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtdcnbleny.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtyfwkuyxt.html

[R19] 数组长度
来源：http://hz.smart0.xyz/gtjilfnxte.html

echo "${#arr[@]}"
来源：http://hz.pycfn.com/gtyxylbycy.html

[R20] 关联数组（字典）
来源：http://hz.yangfankeji.com/gtcfhzunrp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.cashguo.top/gtfkjijoav.html

[R21] 字符串长度
来源：http://hz.chenlongwang.top/gtkmzjtyxd.html

echo "${#s}"
来源：http://hz.cheryme.top/gtvfozjqif.html

[R22] 截取子串
来源：http://hz.jinghuilouyu.cn/gtltevkxsb.html

echo "${s:0:5}"
来源：http://hz.yvedp.cn/gtxqkozcpo.html

[R23] 字符串替换
来源：http://hz.shangyingyoupin.top/gtfymzpvqb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.0kj1m.cn/gtbxlclrzw.html

[R24] 大小写转换
来源：http://hz.c1oappe.top/gtiomwgiak.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.sufxvd.cn/gtsvzyyixm.html

[R25] 去后缀 / 去前缀
来源：http://hz.haohaochexian.top/gtdeziioah.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.cashguo.top/gtcikbiewq.html

[R26] 命令替换
来源：http://hz.sxryk.cn/gtczbcmnvd.html

now=$(date +%F); echo "$now"
来源：http://hz.hywenlv.cn/gtkqcbrccc.html

[R27] 算术展开
来源：http://hz.nanxinkj.top/gtvyyxhnwb.html

echo $((1 + 2 * 3))
来源：http://hz.zycfv.cn/gtpzwpsqto.html

[R28] 浮点运算
来源：http://hz.0kj1m.cn/gtzpvignql.html

echo "scale=2; 10/3" | bc
来源：http://hz.mhx1999.top/gtgziviocd.html

[R29] 定义函数
来源：http://hz.aizwys.cn/gtyotacvos.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sxryk.cn/gthbhjlghk.html

[R30] 函数返回状态码
来源：http://hz.cheryme.top/gtfjhkubzf.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yangfankeji.com/gtejmhkqdy.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtnhlvvzea.html

f() { local x=1; echo "$x"; }
来源：http://hz.zhixingplan.top/gtewebyoas.html

[R32] 参数个数校验
来源：http://hz.aibaodan.cn/gtktbulwfs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenzaomai.com/gttfaritxz.html

[R33] 捕获错误并提示行号
来源：http://hz.jyoumei.cn/gtocrdubsq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.zhixingplan.top/gthjbsmvlg.html

[R34] 退出时清理
来源：http://hz.snrcjt.cn/gtqzxwbfgz.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.yonumen.top/gtilxmnfjn.html

[R35] 后台执行并等待
来源：http://hz.jlsjyb.cn/gtfxdqwthz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.ywan-chungtsiang.top/gtjkclvbay.html

[R36] 并发执行多个任务
来源：http://hz.snrcjt.cn/gtkulviqoo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.xziqi.cn/gtfbaktknp.html

[R37] 把输出赋给变量
来源：http://hz.chenzaomai.com/gtmirnziqp.html

files=$(ls -1)
来源：http://hz.yanxiufei.cn/gtmujrzoeb.html

[R38] 管道串联
来源：http://hz.ehwqpu.com/gtypbqvxjm.html

cat a.txt | grep -i error | wc -l
来源：http://hz.zhongyouzk.top/gtaucpoyoe.html

[R39] 重定向标准输出与错误
来源：http://hz.shuidangran.top/gtqwpvfabn.html

cmd > out.log 2>&1
来源：http://hz.ehwqpu.com/gtplxounaq.html

[R40] 追加写日志
来源：http://hz.guannengcc.top/gtiiwkwbsf.html

echo "log" >> out.log
来源：http://hz.zhixingplan.top/gtqpilrzqe.html

[R41] 丢弃输出
来源：http://hz.pycfn.com/gtifmzylfa.html

cmd >/dev/null 2>&1
来源：http://hz.fengsongda.top/gtwcidmwtu.html

[R42] 输入重定向
来源：http://hz.hammf.cn/gtsktqpeyw.html

wc -l < a.txt
来源：http://hz.chenjidiqi.icu/gtgaqcmdbl.html

[R43] 按名字查找文件
来源：http://hz.vqdsnc.cn/gtcpbczjyc.html

find . -name "*.log" -type f
来源：http://hz.wangshuangyany.cn/gtejxaqbuq.html

[R44] 按修改时间查找
来源：http://hz.gaohongyu789.top/gttuyvsgla.html

find . -mtime -7 -type f
来源：http://hz.yonumen.top/gteifvjhwf.html

[R45] 批量删除
来源：http://hz.sweek.top/gtegjeqlwy.html

find . -name "*.tmp" -delete
来源：http://hz.jinghuilouyu.cn/gtycgkuebw.html

[R46] 递归替换文件内容
来源：http://hz.cdnleiting.top/gtbjrladff.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.iojbl.cn/gtalrtoein.html

[R47] sed 单行替换
来源：http://hz.ppjwa.cn/gtfkwnspnp.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.andypj.xyz/gtwqiesfzs.html

[R48] awk 取指定列
来源：http://hz.hnqzz.top/gtfrhiaept.html

awk '{print $1, $3}' a.txt
来源：http://hz.dianchejie.cn/gtnzknirzl.html

[R49] awk 带条件
来源：http://hz.jqgfzy.top/gtveidrfkm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.ydjk.org.cn/gtddkyazgq.html

[R50] awk 求和
来源：http://hz.zhiwuduotai.top/gtolkwsqxw.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.0kj1m.cn/gttkcgksad.html

[R51] 排序去重取前几
来源：http://hz.yonumen.top/gtsaxulwiy.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.chenzaomai.com/gtljaxphha.html

[R52] 统计行数
来源：http://hz.zhoulong.xyz/gtuhiiohcw.html

wc -l a.txt
来源：http://hz.jinqigufen.top/gtewtjzwob.html

[R53] 查看文件头与实时尾
来源：http://hz.aibaodan.cn/gtxvrcegsb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.zdqjudy.top/gtyxnylpyo.html

[R54] 比较两个文件
来源：http://hz.hywenlv.cn/gtcoecglka.html

diff a.txt b.txt
来源：http://hz.guannengcc.top/gttmbnnbdh.html

[R55] 压缩与解压
来源：http://hz.zhixingplan.top/gtqysqijqg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.pycfn.com/gtwfqchbet.html

[R56] 远程拷贝
来源：http://hz.smart0.xyz/gtuerapqgc.html

scp file user@host:/path/
来源：http://hz.dashuyun.cn/gtcfxpdxoz.html

[R57] 远程执行命令
来源：http://hz.snrcjt.cn/gtnnlcyocq.html

ssh user@host 'uptime'
来源：http://hz.andypj.xyz/gtkfmbplzg.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gttlfzmzab.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xuanzx.com/gtzbrqfbum.html

[R59] 发 POST JSON
来源：http://hz.sweek.top/gtvlnmmonf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yongpay.top/gtfqkvxzjm.html

[R60] 只看 HTTP 状态码
来源：http://hz.svipenyu.cn/gtkomheccd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.kuanghao11.cn/gtfezhmjqg.html

[R61] 磁盘占用
来源：http://hz.yangfankeji.com/gtqstgzdco.html

df -h;  du -sh *
来源：http://hz.xinyue.icu/gtsuupybcb.html

[R62] 找最占空间的文件
来源：http://hz.shanyushiyangtech.top/gtdukiwnds.html

du -ah . | sort -rh | head -10
来源：http://hz.aibaodan.cn/gtxpsfhgjm.html

[R63] 内存与进程
来源：http://hz.cqqwz.cn/gtowykompg.html

free -h;  ps aux | grep nginx
来源：http://hz.jqgufenzy.top/gtcgycyukv.html

[R64] 结束进程
来源：http://hz.yj202588.top/gtrnbcsjhl.html

kill -9 $(pgrep -f app.py)
来源：http://hz.chenjidiqi.icu/gtscmbbwor.html

[R65] 查看端口占用
来源：http://hz.jyoumei.cn/gtnppsbxed.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.gaohongyu789.top/gtdzaorzdk.html

[R66] 定时任务
来源：http://hz.ehwqpu.com/gtbiqagwft.html

crontab -e;  crontab -l
来源：http://hz.cqqwz.cn/gtuxxxwgzy.html

[R67] 生成随机十六进制串
来源：http://hz.havefunace.top/gtejqgjsbu.html

openssl rand -hex 16
来源：http://hz.nanxuanxn.top/gtcmzixnyg.html

[R68] 计算文件校验值
来源：http://hz.yangfankeji.com/gtvdilpnon.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yj202588.top/gtepcenjgf.html

[R69] 生成随机密码
来源：http://hz.shangyingyoupin.top/gtvvagqbsi.html

head -c 16 /dev/urandom | base64
来源：http://hz.redwolf501.top/gtqsedzdht.html

[R70] 时间戳与互转
来源：http://hz.zhaomingkeji.xyz/gttbvzyfwy.html

date +%s;  date -d @1700000000
来源：http://hz.jiagoushi.top/gtniyweysg.html

[R71] 日期格式化
来源：http://hz.aibaodan.cn/gtxsfvbtaj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtrovnuaxy.html

[R72] 等待端口就绪
来源：http://hz.ywan-chungtsiang.top/gtvfaufjpl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sweek.top/gtcdkukjib.html

[R73] 分割大日志
来源：http://hz.quarkkingdee.top/gtcoiweoio.html

split -l 1000 big.log part_
来源：http://hz.chenlongwang.top/gtnmgsldqn.html

[R74] 批量重命名
来源：http://hz.birdmap.top/gtdnzfxijk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.smart0.xyz/gtzvqqxfsu.html

[R75] 导出环境变量
来源：http://hz.dianchejie.cn/gtwvgypjol.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.zhiwuduotai.top/gtoldhhrqk.html

[R76] 使用临时文件
来源：http://hz.aibaodan.cn/gtideddnot.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.yvedp.cn/gtytxtabxx.html

[R77] 读取用户输入
来源：http://hz.yangfankeji.com/gtojqbxpif.html

read -rp "请输入: " ans
来源：http://hz.ehwqpu.com/gtlhdqwdrv.html

[R78] 交互式菜单
来源：http://hz.sxryk.cn/gtrankpphq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhengqikj.top/gttxfufika.html

[R79] 解析命令行选项
来源：http://hz.chenlongwang.top/gtuwbacupx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.ydzc1.top/gtxbnmagag.html

[R80] 查看脚本执行耗时
来源：http://hz.shangyingyoupin.top/gtzlawfshm.html

time ./run.sh
来源：http://hz.yvedp.cn/gthofsggzt.html

================================================================================
来源：http://hz.nanxinkj.top/gtoouzwebn.html

S. C / C++ 专题
来源：http://hz.redwolf501.top/gtkjqoqeao.html

================================================================================
来源：http://hz.zhongyouzk.top/gtfesqptse.html

[S01] C：Hello World
来源：http://hz.iojbl.cn/gtrqbfavnp.html

#include <stdio.h>
来源：http://hz.xylfe.cn/gtqmyyapns.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj202588.top/gtyhzjqgly.html

[S02] C：变量与格式化输出
来源：http://hz.c1oappe.top/gtwfmlevet.html

int a = 10; printf("%d\n", a);
来源：http://hz.hammf.cn/gtucvprgiw.html

[S03] C：读入整数
来源：http://hz.meibo888.top/gtmhwjgwkp.html

int x; scanf("%d", &x);
来源：http://hz.mhx1999.top/gtrfwskknr.html

[S04] C：字符串复制
来源：http://hz.52xcode.cn/gtpgvdxfdp.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jianghu66.top/gtdgakxnnb.html

[S05] C：字符串长度
来源：http://hz.hammf.cn/gtdjmbrfvn.html

strlen(s)
来源：http://hz.zhoulong.xyz/gtcxksemua.html

[S06] C：字符串比较
来源：http://hz.zhixingplan.top/gtxxntlxyq.html

strcmp(a, b) == 0
来源：http://hz.shanyushiyangkeji.top/gtufcnvocy.html

[S07] C：数组遍历求和
来源：http://hz.nanxinkj.top/gtxpoxuyzy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.daria6918.cn/gtfzakxnod.html

[S08] C：动态内存分配与释放
来源：http://hz.guannengcc.top/gtudvxprnk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jiagoushi.top/gtyoodgxjc.html

[S09] C：结构体定义与初始化
来源：http://hz.hfpthk.cn/gtiovjrkld.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.smart0.xyz/gtlupqcwct.html

[S10] C：指针与解引用
来源：http://hz.gzhubu.top/gticcnltrm.html

int *p = &a;  *p = 5;
来源：http://hz.sxryk.cn/gtthunbxax.html

[S11] C：逐行读文件
来源：http://hz.yongpay.top/gtzdopxttb.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.wangdashe.top/gtcfxirsdk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.cashguo.top/gttrkssaqs.html

fclose(f);
来源：http://hz.52xcode.cn/gtiwpfofap.html

[S12] C：写文件
来源：http://hz.daxiang520.top/gtgllincam.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.chenjidiqi.icu/gtscqivjwi.html

[S13] C：宏定义
来源：http://hz.gzhubu.top/gtijfzspjt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.yuxming.cn/gtpcwhavbh.html

[S14] C：枚举
来源：http://hz.jinqigufen.top/gtmbtxezbu.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.xylfe.cn/gtiwdqkjzc.html

[S15] C：类型转换
来源：http://hz.hnqzz.top/gtxavqypuk.html

(double) a / b
来源：http://hz.jinqigufen.top/gtsxluobin.html

[S16] C：位操作置位
来源：http://hz.zhaomingkeji.xyz/gtgwgvbyrn.html

x |= (1 << 3);
来源：http://hz.smart0.xyz/gtfxrlztaq.html

[S17] C：安全拼接字符串
来源：http://hz.dianchejie.cn/gtczwlikvy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.chenlongwang.top/gtzakdmdmq.html

[S18] C：命令行参数
来源：http://hz.yj20258888.top/gtuodinbfy.html

int main(int argc, char **argv)
来源：http://hz.ehwqpu.com/gtwcdfkrjk.html

[S19] C：快速排序
来源：http://hz.jinghuilouyu.cn/gteobyuspq.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.xziqi.cn/gtcwcpeuyf.html

[S20] C：二分查找
来源：http://hz.cashguo.top/gtvlkfswtt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.birdmap.top/gtwnapjdnf.html

[S21] C：字符类别判断
来源：http://hz.xuanzx.com/gtifuauvlv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yj20258888.top/gtfmycftha.html

[S22] C：字符串转数字
来源：http://hz.cqqwz.cn/gtbcpthksw.html


<!-- 参考信息 -->