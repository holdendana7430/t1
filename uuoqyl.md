代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.yuxming.cn/gtkmeulwdx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.meibo888.top/gtrjawlukn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.zhijiandao.cn/gtbrmpbhft.html

[Q41] 多表连接
来源：http://hz.sxryk.cn/gtoptadhvw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.ywan-chungtsiang.top/gtgkfhfxpg.html

JOIN users u ON u.id = o.user_id
来源：http://hz.jinghuilouyu.cn/gtgxefkfme.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.zycfv.cn/gtmikqmjcj.html

[Q42] 连接条件附加过滤
来源：http://hz.ydjk.org.cn/gtvsosboxr.html

SELECT u.name, o.amount FROM users u
来源：http://hz.zhoulong.xyz/gtaqlzslas.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.nanxuanxn.top/gtkuofuxcu.html

[Q43] 标量子查询
来源：http://hz.shangyingyoupin.top/gtooaopsiv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.yueranfly.top/gtnldvrztk.html

[Q44] IN 子查询
来源：http://hz.bjfxy.top/gtvfqicnvd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinqigfzy.top/gtchdelahl.html

[Q45] EXISTS 判断存在
来源：http://hz.jqgufenzy.top/gtzuamvrsm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.redwolf501.top/gtosuyhfaa.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.xziqi.cn/gtkgkarowe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.gogol.net.cn/gthavyxagd.html

[Q47] 与平均值比较
来源：http://hz.guowangkeji.top/gtvxmaquua.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.hammf.cn/gtmvxuzhlt.html

[Q48] CTE 公用表表达式
来源：http://hz.cheryme.top/gtspxmkzqa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.chenlongwang.top/gtmacloczm.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.hfpthk.cn/gtimptkayi.html

[Q49] 更新单行
来源：http://hz.cashguo.top/gtaucezmwa.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.quarkkingdee.top/gtkbblynsv.html

[Q50] 批量更新
来源：http://hz.yongpay.top/gtyloiduqy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.jinghuilouyu.cn/gtuifrpsru.html

[Q51] 用子查询更新
来源：http://hz.fzhhl.top/gtcdwzfxwe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.yuanzhike.top/gtqfcxvtqa.html

[Q52] 删除指定行
来源：http://hz.jinghuilouyu.cn/gtswfmubyb.html

DELETE FROM users WHERE id = 10;
来源：http://hz.ydzc1.top/gtdfvwaadz.html

[Q53] 按条件删除
来源：http://hz.gaohongyu789.top/gtdtaqxxgd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.shanyushiyangkeji.top/gtcnznapty.html

[Q54] 清空表
来源：http://hz.9152youxi.cn/gtrdahzuwv.html

TRUNCATE TABLE logs;
来源：http://hz.chenzaomai.com/gtqheygurg.html

[Q55] 排名（并列占位）
来源：http://hz.smart0.xyz/gtamhsfswi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.guannengcc.top/gtpjlxsxev.html

[Q56] 密集排名（并列不占位）
来源：http://hz.zhixingplan.top/gtohiepnwl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtyvbmwbjx.html

[Q57] 行号
来源：http://hz.svipenyu.cn/gtvewqjmai.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.xuetiantiany.cn/gtnzrbufqy.html

[Q58] 累计求和
来源：http://hz.yuanzhike.top/gtadarocyo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.ybcxt.top/gtynyydywg.html

[Q59] 分组内累计
来源：http://hz.yonumen.top/gtwxiupuvo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.yangfankeji.com/gtvkqphxzk.html

[Q60] 取上一行 / 下一行
来源：http://hz.wangshuangyany.cn/gtfmyiubeh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.ehwqpu.com/gtlmtosflt.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.sysykeji.top/gtwpnopkby.html

[Q61] 移动平均
来源：http://hz.cheryme.top/gtwtvvibjp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.zhengqikj.top/gtqtrscpsc.html

[Q62] 分组占比
来源：http://hz.wangdashe.top/gtwnsnhpxg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.yuxming.cn/gtvyzmoxvu.html

[Q63] 开启事务
来源：http://hz.andypj.xyz/gtweuxhnng.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.hysaishi.cn/gtqkqqqvhk.html

[Q64] 提交事务
来源：http://hz.dianchejie.cn/gtxzizibge.html

COMMIT;
来源：http://hz.nanxuanxn.top/gtkwzyhfbm.html

[Q65] 回滚事务
来源：http://hz.jqgfzy.top/gtoscjglnx.html

ROLLBACK;
来源：http://hz.nanxinkj.top/gtppdigpvd.html

[Q66] 行锁查询
来源：http://hz.wangdashe.top/gtbpusxbzn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.daria6918.cn/gtrfwbzryx.html

[Q67] 设置隔离级别
来源：http://hz.ywan-chungtsiang.top/gtzrlrzzam.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.tian-w.cn/gtntzqlkkd.html

[Q68] 保存点
来源：http://hz.zhengqikj.top/gtcziybwjl.html

SAVEPOINT sp1;
来源：http://hz.daxiang520.top/gtqomifogo.html

ROLLBACK TO sp1;
来源：http://hz.zycfv.cn/gtcmddquzw.html

[Q69] 查看执行计划
来源：http://hz.wangdashe.top/gtcbwoarlm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.fzhhl.top/gtnjgadkxr.html

[Q70] 更新统计信息
来源：http://hz.tian-w.cn/gthslljxeo.html

ANALYZE TABLE users;
来源：http://hz.hnxiangtu.top/gtcxeunjcs.html

[Q71] 查看建表语句
来源：http://hz.shuidangran.top/gtweahzqqu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.hnqzz.top/gtsdpbrpjl.html

[Q72] 查看索引
来源：http://hz.yuxming.cn/gttucfqzld.html

SHOW INDEX FROM users;
来源：http://hz.snrcjt.cn/gtsavmkymu.html

[Q73] 查看表状态
来源：http://hz.nanxuanxn.top/gtbrovobtw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.wangdashe.top/gtykqsvozo.html

[Q74] 强制使用索引
来源：http://hz.quarkkingdee.top/gtgyxnnuvd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.yueranfly.top/gtrorjdocy.html

[Q75] 日期格式化
来源：http://hz.nanxinkj.top/gtgspitevp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.yj202588.top/gtfpyiyhrp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.fengsongda.top/gtpuiokzgi.html

[Q76] 按天统计
来源：http://hz.gaohongyu789.top/gtmknaggvb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shuidangran.top/gtxtqnebsq.html

[Q77] 时间加减
来源：http://hz.cashguo.top/gtiiwmdxzo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sysykeji.top/gtkrhefohr.html

[Q78] 当前时间
来源：http://hz.xingfuxueyuan.xyz/gtcnsyjeoj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.tianlin.xyz/gtfrozfkih.html

[Q79] 字符串拼接
来源：http://hz.havefunace.top/gtcbdjmlhe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cheryme.top/gtyuxbrvxa.html

[Q80] 字符串截取
来源：http://hz.zhiwuduotai.top/gtxgysbmxm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.wangshuangyany.cn/gtvkflfdpy.html

[Q81] 字符串替换
来源：http://hz.jinghuilouyu.cn/gtsapfnjiy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.gaohongyu789.top/gtxlsdqnbd.html

[Q82] 字符长度与字节长度
来源：http://hz.fengsongda.top/gtxlvqcgds.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zycfv.cn/gtpgwyygeq.html

[Q83] 大小写转换
来源：http://hz.xziqi.cn/gthdnummom.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.andypj.xyz/gtnbzszola.html

[Q84] 去除首尾空格
来源：http://hz.yj202588.top/gtcvtygyil.html

SELECT TRIM(name) FROM users;
来源：http://hz.dianchejie.cn/gtqplkkdud.html

[Q85] 数值取整
来源：http://hz.yj20258.top/gtuarqxefb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.yj20258.top/gtunqhlmym.html

[Q86] 读取 JSON 字段
来源：http://hz.jyoumei.cn/gtmgyszfln.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.sysykeji.top/gtidpmhlsh.html

[Q87] JSON 字段做条件
来源：http://hz.ydzc1.top/gtcaadkulv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.hfpthk.cn/gtyobaqkud.html

[Q88] 行转列（条件聚合）
来源：http://hz.yanxiufei.cn/gtjsuzspjq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.xuanzx.com/gtryohpika.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnqzz.top/gtviioletf.html

[Q89] 判断表是否存在
来源：http://hz.gzhubu.top/gtxtesccvh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.hfpthk.cn/gthurnxzos.html

[Q90] 生成序号列
来源：http://hz.pengpengdd.cyou/gtlzsrornr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.0kj1m.cn/gtqvxowhln.html

================================================================================
来源：http://hz.hnqzz.top/gtovvxwitf.html

R. Bash 专题
来源：http://hz.daxiang520.top/gtdntvhwfc.html

================================================================================
来源：http://hz.chenzaomai.com/gtvldtxffp.html

[R01] shebang 与严格模式
来源：http://hz.zhijiandao.cn/gtojzpwavz.html

#!/usr/bin/env bash
来源：http://hz.hnqzz.top/gtcgiomaqx.html

set -euo pipefail
来源：http://hz.yj20258.top/gtjrjrdmiv.html

[R02] 变量赋值与使用
来源：http://hz.birdmap.top/gtavrzxpgq.html

name="Tom"; echo "$name"
来源：http://hz.ywan-chungtsiang.top/gtxyxkbhrl.html

[R03] 只读变量
来源：http://hz.bjfxy.top/gtljsvfzwn.html

readonly PI=3.14
来源：http://hz.iojbl.cn/gtnezegtkw.html

[R04] 位置参数
来源：http://hz.aibaodan.cn/gtygbcjxuj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yj202588.top/gtivsogaff.html

[R05] 参数默认值
来源：http://hz.pengpengdd.cyou/gthclngolf.html

name="${1:-default}"
来源：http://hz.chenlongwang.top/gtkbnqvwfw.html

[R06] 判断命令是否存在
来源：http://hz.yonumen.top/gtfdexjhio.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.fengsongda.top/gtqnyivcnl.html

[R07] if 判断文件
来源：http://hz.xinyue.icu/gtswkbbfrh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.xingfuxueyuan.xyz/gtebrbilxm.html

[R08] 数值比较
来源：http://hz.bjfxy.top/gtfepblnzr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.havefunace.top/gtnkhdgcur.html

[R09] 字符串比较
来源：http://hz.jqgufenzy.top/gtekylvbin.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.svipenyu.cn/gtbymbykiv.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtmwhqhbrz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.zhoulong.xyz/gtfixqozko.html

[R11] case 多分支
来源：http://hz.havefunace.top/gtvwjjqhch.html

case "$1" in
来源：http://hz.fengsongda.top/gtaoadnefj.html

start) echo "启动" ;;
来源：http://hz.c1oappe.top/gtklpmxoia.html

stop)  echo "停止" ;;
来源：http://hz.havefunace.top/gtihzsfbci.html

*)     echo "未知命令" ;;
来源：http://hz.zhengqikj.top/gtrzkpkxjb.html

esac
来源：http://hz.zhixingplan.top/gtzriomiim.html

[R12] for 遍历文件
来源：http://hz.dashuyun.cn/gttuveaxib.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shangyingyoupin.top/gtlpnskmip.html

[R13] for 计数循环
来源：http://hz.chenzaomai.com/gtwjpdfbxv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.hfpthk.cn/gtwkinkqqu.html

[R14] C 风格 for
来源：http://hz.jinqigufen.top/gtxhitiblq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.havefunace.top/gtnxnczvgr.html

[R15] while 逐行读文件
来源：http://hz.feifeiyinyue.top/gtcpqkzmnt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.gzhubu.top/gtsatraoye.html

[R16] until 等待条件
来源：http://hz.yj202588.top/gtaztqiziw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.jyoumei.cn/gtsrzcvolv.html

[R17] 数组定义与取值
来源：http://hz.chenjidiqi.icu/gtdniszdyh.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.cucudq.cn/gtjjvxlorh.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gtvdxirmkn.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.hnxiangtu.top/gttygritby.html

[R19] 数组长度
来源：http://hz.iojbl.cn/gtbieforfr.html

echo "${#arr[@]}"
来源：http://hz.nwbrower.top/gthbbcrcog.html

[R20] 关联数组（字典）
来源：http://hz.fzhhl.top/gtrhawpcnp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.hongshengwenyu.top/gtpypkwdts.html

[R21] 字符串长度
来源：http://hz.hnqzz.top/gtbwaelqub.html

echo "${#s}"
来源：http://hz.gzhubu.top/gturpxwmtt.html

[R22] 截取子串
来源：http://hz.ivvv.top/gtcrttkprx.html

echo "${s:0:5}"
来源：http://hz.wangshuangyany.cn/gtxjbknvjf.html

[R23] 字符串替换
来源：http://hz.zhaomingkeji.xyz/gtcesujkms.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.c1oappe.top/gthnyyvrtr.html

[R24] 大小写转换
来源：http://hz.9152youxi.cn/gtvhtzfdnb.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.iojbl.cn/gtqymrgvwn.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydzc1.top/gtfpysuzeo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.tianlin.xyz/gtzwqkdpcs.html

[R26] 命令替换
来源：http://hz.ppjwa.cn/gtnxkuofbi.html

now=$(date +%F); echo "$now"
来源：http://hz.yuanzhike.top/gtiuseyygn.html

[R27] 算术展开
来源：http://hz.yj20258.top/gtggvfiypm.html

echo $((1 + 2 * 3))
来源：http://hz.ydzc1.top/gtgdtsmqra.html

[R28] 浮点运算
来源：http://hz.shanyushiyangtech.top/gtondmyopt.html

echo "scale=2; 10/3" | bc
来源：http://hz.gaohongyu789.top/gtrkzrbikx.html

[R29] 定义函数
来源：http://hz.cheryme.top/gttvyggnmm.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yuanzhike.top/gtucikeqbe.html

[R30] 函数返回状态码
来源：http://hz.dashuyun.cn/gtnyteqofa.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.cdnleiting.top/gtazlqadfp.html

[R31] 局部变量
来源：http://hz.cqqwz.cn/gtihoctsap.html

f() { local x=1; echo "$x"; }
来源：http://hz.snrcjt.cn/gtqkwifupg.html

[R32] 参数个数校验
来源：http://hz.kuanghao11.cn/gtkrtrwzoa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.yj20258888.top/gtxsdvapdv.html

[R33] 捕获错误并提示行号
来源：http://hz.snrcjt.cn/gthdzvyhln.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.iojbl.cn/gtjkxgcypk.html

[R34] 退出时清理
来源：http://hz.zycfv.cn/gtabjiibzr.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.aizwys.cn/gtjvpdpewj.html

[R35] 后台执行并等待
来源：http://hz.sufxvd.cn/gtzcfiejab.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.jiagoushi.top/gtcjitzcec.html

[R36] 并发执行多个任务
来源：http://hz.mhx1999.top/gtpfqpgnol.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.sweek.top/gtlnsaijsx.html

[R37] 把输出赋给变量
来源：http://hz.yonumen.top/gtogavimjn.html

files=$(ls -1)
来源：http://hz.gaohongyu789.top/gtcrqhhwjh.html

[R38] 管道串联
来源：http://hz.jinqigufen.top/gtezjihkqk.html

cat a.txt | grep -i error | wc -l
来源：http://hz.guowangkeji.top/gtzxwbwzuu.html

[R39] 重定向标准输出与错误
来源：http://hz.chenjidiqi.icu/gtejsuiqhf.html

cmd > out.log 2>&1
来源：http://hz.sweek.top/gtjjpcaozq.html

[R40] 追加写日志
来源：http://hz.yj20258.top/gtdrhsfaah.html

echo "log" >> out.log
来源：http://hz.jqgfzy.top/gtkjfouvff.html

[R41] 丢弃输出
来源：http://hz.yanxiufei.cn/gtgjagokih.html

cmd >/dev/null 2>&1
来源：http://hz.xinyue.icu/gtvpanfqma.html

[R42] 输入重定向
来源：http://hz.hfpthk.cn/gtkcyqmlat.html

wc -l < a.txt
来源：http://hz.pycfn.com/gtccjnynms.html

[R43] 按名字查找文件
来源：http://hz.hysaishi.cn/gtfyshwiug.html

find . -name "*.log" -type f
来源：http://hz.ehwqpu.com/gtlvrejrgf.html

[R44] 按修改时间查找
来源：http://hz.kuanghao11.cn/gtgoapsfzh.html

find . -mtime -7 -type f
来源：http://hz.sweek.top/gtzqchemoj.html

[R45] 批量删除
来源：http://hz.yvedp.cn/gtvsjglbga.html

find . -name "*.tmp" -delete
来源：http://hz.jyoumei.cn/gtyhwyiwaj.html

[R46] 递归替换文件内容
来源：http://hz.guannengcc.top/gtoihucxtl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.fengsongda.top/gthryuyqtc.html

[R47] sed 单行替换
来源：http://hz.aizwys.cn/gtjoldmwtm.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.mhx1999.top/gtggeblulc.html

[R48] awk 取指定列
来源：http://hz.zhixingplan.top/gtshfwqeyr.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtezyaplvj.html

[R49] awk 带条件
来源：http://hz.jyoumei.cn/gtqkqpzxox.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.xingfuxueyuan.xyz/gtoibuzbkd.html

[R50] awk 求和
来源：http://hz.c1oappe.top/gtysidebpq.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.hnqzz.top/gtqpqmdlqz.html

[R51] 排序去重取前几
来源：http://hz.kuanghao11.cn/gtiwkfljbx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ybcxt.top/gtmyvosrxp.html

[R52] 统计行数
来源：http://hz.daxiang520.top/gtbffvqvsn.html

wc -l a.txt
来源：http://hz.jlsjyb.cn/gtlvuoewga.html

[R53] 查看文件头与实时尾
来源：http://hz.feifeiyinyue.top/gtjjptcens.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jinyuanbaomall.cn/gtbrrjnvfp.html

[R54] 比较两个文件
来源：http://hz.hfpthk.cn/gtjentifmj.html

diff a.txt b.txt
来源：http://hz.birdmap.top/gtxmkmtuov.html

[R55] 压缩与解压
来源：http://hz.hnqzz.top/gtclnrfmdi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.jinghuilouyu.cn/gtcsudjcdz.html

[R56] 远程拷贝
来源：http://hz.sufxvd.cn/gtphpugohm.html

scp file user@host:/path/
来源：http://hz.ybcxt.top/gtvecrfpdm.html

[R57] 远程执行命令
来源：http://hz.jinqigufen.top/gtvmohzyjh.html

ssh user@host 'uptime'
来源：http://hz.yangfankeji.com/gthkdsggfz.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtlcokhwpa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.cdnleiting.top/gtgoyginve.html

[R59] 发 POST JSON
来源：http://hz.wangdashe.top/gtxbtlqgti.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.chenzaomai.com/gtxgpqbzrv.html

[R60] 只看 HTTP 状态码
来源：http://hz.yj20258.top/gthibpcfux.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.cheryme.top/gtsawmcvvm.html

[R61] 磁盘占用
来源：http://hz.zhixingplan.top/gtaliryzvp.html

df -h;  du -sh *
来源：http://hz.sxryk.cn/gtikaiuhwn.html

[R62] 找最占空间的文件
来源：http://hz.gotoacloud.top/gtvrdfthod.html

du -ah . | sort -rh | head -10
来源：http://hz.xziqi.cn/gtbntotuvk.html

[R63] 内存与进程
来源：http://hz.hongshengwenyu.top/gticukvgsb.html

free -h;  ps aux | grep nginx
来源：http://hz.shangyingyoupin.top/gtavhbuwfu.html

[R64] 结束进程
来源：http://hz.wangdashe.top/gtbumayjvt.html

kill -9 $(pgrep -f app.py)
来源：http://hz.havefunace.top/gtojqmyahf.html

[R65] 查看端口占用
来源：http://hz.bjfxy.top/gtszxnhqiq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.jinqigufen.top/gtmklqzctl.html

[R66] 定时任务
来源：http://hz.yvedp.cn/gtzmwlwjvg.html

crontab -e;  crontab -l
来源：http://hz.hnxiangtu.top/gtftqsgika.html

[R67] 生成随机十六进制串
来源：http://hz.birdmap.top/gtopcthria.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gtpzrikrbx.html

[R68] 计算文件校验值
来源：http://hz.cdnleiting.top/gtscxummcq.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.yvedp.cn/gtqnimpjdp.html

[R69] 生成随机密码
来源：http://hz.jinghuilouyu.cn/gtspadybjh.html

head -c 16 /dev/urandom | base64
来源：http://hz.9152youxi.cn/gtxeerglhx.html

[R70] 时间戳与互转
来源：http://hz.cdnleiting.top/gtovvgbrrn.html

date +%s;  date -d @1700000000
来源：http://hz.yj20258888.top/gtywejzpjr.html

[R71] 日期格式化
来源：http://hz.chenjidiqi.icu/gtibxptayd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.shzxlz.cn/gtrzizriwa.html

[R72] 等待端口就绪
来源：http://hz.zycfv.cn/gtpxqsucqd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.xziqi.cn/gtmbxzvfhb.html

[R73] 分割大日志
来源：http://hz.zhixingplan.top/gtrmorikme.html

split -l 1000 big.log part_
来源：http://hz.dashuyun.cn/gtgmmtbhud.html

[R74] 批量重命名
来源：http://hz.xuetiantiany.cn/gtjvsuwstk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinqigfzy.top/gtxoqbhiol.html

[R75] 导出环境变量
来源：http://hz.xuetiantiany.cn/gtknhmnmit.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.svipenyu.cn/gtxrnxmepb.html

[R76] 使用临时文件
来源：http://hz.feifeiyinyue.top/gtsadbxqua.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.jinqigfzy.top/gthcnthdfq.html

[R77] 读取用户输入
来源：http://hz.shanyushiyangkeji.top/gtriawzuxn.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gtpgwkppjq.html

[R78] 交互式菜单
来源：http://hz.jinyuanbaomall.cn/gtvooqtonx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.zhoulong.xyz/gtnvpvvzft.html

[R79] 解析命令行选项
来源：http://hz.0kj1m.cn/gtsshdwrds.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.0kj1m.cn/gtfosedvjd.html

[R80] 查看脚本执行耗时
来源：http://hz.52xcode.cn/gtbeyyeavh.html

time ./run.sh
来源：http://hz.iojbl.cn/gtxmriopgy.html

================================================================================
来源：http://hz.svipenyu.cn/gtwqwtbqdg.html

S. C / C++ 专题
来源：http://hz.bjfxy.top/gtuiuachdr.html

================================================================================
来源：http://hz.redwolf501.top/gtxnvjlcpk.html

[S01] C：Hello World
来源：http://hz.birdmap.top/gtgsqdmleu.html

#include <stdio.h>
来源：http://hz.quarkkingdee.top/gtkabdgjuk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.zhiwuduotai.top/gtzialffxe.html

[S02] C：变量与格式化输出
来源：http://hz.shangyingyoupin.top/gtbxbxfxvf.html

int a = 10; printf("%d\n", a);
来源：http://hz.kuanghao11.cn/gtjotaalyh.html

[S03] C：读入整数
来源：http://hz.0kj1m.cn/gtfmyffknl.html

int x; scanf("%d", &x);
来源：http://hz.tianlin.xyz/gticfddcex.html

[S04] C：字符串复制
来源：http://hz.jinyuanbaomall.cn/gtzechmzok.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.yanxiufei.cn/gtssjedpvu.html

[S05] C：字符串长度
来源：http://hz.0kj1m.cn/gtwwhisxgk.html

strlen(s)
来源：http://hz.yj20258.top/gtoyeuuhbm.html

[S06] C：字符串比较
来源：http://hz.dianchejie.cn/gtaqgskgpj.html

strcmp(a, b) == 0
来源：http://hz.ydzc1.top/gtatjsjuuf.html

[S07] C：数组遍历求和
来源：http://hz.jiagoushi.top/gtonxwqpaq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.pycfn.com/gtbpgaywzm.html

[S08] C：动态内存分配与释放
来源：http://hz.aizwys.cn/gtcwnpeswl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.pycfn.com/gtnenkqiye.html

[S09] C：结构体定义与初始化
来源：http://hz.zhongyouzk.top/gtnsiyldyy.html


<!-- 参考信息 -->