代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.chenzaomai.com/gtzjkbdmft.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.jiagoushi.top/gtxbcvzddn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.pengpengdd.cyou/gtqnjtorbd.html

[Q41] 多表连接
来源：http://hz.guannengcc.top/gtvsgallkv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.gotoacloud.top/gtqgzedwpu.html

JOIN users u ON u.id = o.user_id
来源：http://hz.shangyingyoupin.top/gtvrnkrnbw.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.hnqzz.top/gtkkmxanop.html

[Q42] 连接条件附加过滤
来源：http://hz.shanyushiyangtech.top/gtmybutuqi.html

SELECT u.name, o.amount FROM users u
来源：http://hz.shanyushiyangtech.top/gtwyomhmiw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.shangyingyoupin.top/gtjndgnrjd.html

[Q43] 标量子查询
来源：http://hz.ivvv.top/gtvepjwnns.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.cashguo.top/gtwiwgfnie.html

[Q44] IN 子查询
来源：http://hz.yvedp.cn/gtsszexyop.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jinyuanbaomall.cn/gtjqqszeqc.html

[Q45] EXISTS 判断存在
来源：http://hz.mhx1999.top/gthfxfdlvc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.sxryk.cn/gttaeorgmy.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.ydzc1.top/gtlyubclln.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.yvedp.cn/gttlejohmf.html

[Q47] 与平均值比较
来源：http://hz.yongpay.top/gtdaisydtg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.ydzc1.top/gtyxlixpql.html

[Q48] CTE 公用表表达式
来源：http://hz.sysykeji.top/gtxjagogzl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.fengsongda.top/gtotkeaoxa.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.bjfxy.top/gtgkykpjpe.html

[Q49] 更新单行
来源：http://hz.ehwqpu.com/gtouuwaypb.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.snrcjt.cn/gtslcjmasu.html

[Q50] 批量更新
来源：http://hz.cucudq.cn/gtgumfhcdi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.ydjk.org.cn/gtkpurebon.html

[Q51] 用子查询更新
来源：http://hz.pycfn.com/gtjfvguzon.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.pycfn.com/gtftwrgvoe.html

[Q52] 删除指定行
来源：http://hz.jianghu66.top/gtuetkwsup.html

DELETE FROM users WHERE id = 10;
来源：http://hz.hfpthk.cn/gtvcgrwjhf.html

[Q53] 按条件删除
来源：http://hz.gotoacloud.top/gtxdyyrmmr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.zhoulong.xyz/gtmvsiwutg.html

[Q54] 清空表
来源：http://hz.hywenlv.cn/gtfgdeetuo.html

TRUNCATE TABLE logs;
来源：http://hz.ywan-chungtsiang.top/gtmshcctxx.html

[Q55] 排名（并列占位）
来源：http://hz.zhiwuduotai.top/gtfmhfxkbc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.svipenyu.cn/gttcqtsfpd.html

[Q56] 密集排名（并列不占位）
来源：http://hz.shanyushiyangtech.top/gttmrzdfcg.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.nwbrower.top/gtggwkgkff.html

[Q57] 行号
来源：http://hz.wangshuangyany.cn/gtsutfffiv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zycfv.cn/gtacgsuvki.html

[Q58] 累计求和
来源：http://hz.pengpengdd.cyou/gtcqsyumtv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.cqqwz.cn/gtxpdykjfb.html

[Q59] 分组内累计
来源：http://hz.gotoacloud.top/gtkoedspgh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.redwolf501.top/gtxuemqinn.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gttmfhtsnp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yj20258888.top/gtxlzdfizr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.zycfv.cn/gtyjirbtwn.html

[Q61] 移动平均
来源：http://hz.sxryk.cn/gtgczidalg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.mhx1999.top/gthyfvhnyp.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gthpimuybg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.zhongyouzk.top/gtnsglddwk.html

[Q63] 开启事务
来源：http://hz.dianchejie.cn/gtrjpfmedi.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.daria6918.cn/gtyjwymvnh.html

[Q64] 提交事务
来源：http://hz.hnqzz.top/gtnftelems.html

COMMIT;
来源：http://hz.zhengqikj.top/gtpofmtpwx.html

[Q65] 回滚事务
来源：http://hz.jiagoushi.top/gtljovhllb.html

ROLLBACK;
来源：http://hz.zhaomingkeji.xyz/gteoyrmbkx.html

[Q66] 行锁查询
来源：http://hz.svipenyu.cn/gtyrexicoo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.jinyuanbaomall.cn/gtwllkmonk.html

[Q67] 设置隔离级别
来源：http://hz.svipenyu.cn/gtvbnruuvy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.pycfn.com/gtudfvtqbc.html

[Q68] 保存点
来源：http://hz.havefunace.top/gtoqgmzylb.html

SAVEPOINT sp1;
来源：http://hz.sufxvd.cn/gtfriftcbu.html

ROLLBACK TO sp1;
来源：http://hz.sufxvd.cn/gtamqacjvd.html

[Q69] 查看执行计划
来源：http://hz.jianghu66.top/gtvbparyix.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.wangdashe.top/gtjdihhdpw.html

[Q70] 更新统计信息
来源：http://hz.sxryk.cn/gtqonmlimt.html

ANALYZE TABLE users;
来源：http://hz.0kj1m.cn/gtdvrnelur.html

[Q71] 查看建表语句
来源：http://hz.mhx1999.top/gtslexxrhc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ivvv.top/gtgioypqaq.html

[Q72] 查看索引
来源：http://hz.ppjwa.cn/gtqxtdfrog.html

SHOW INDEX FROM users;
来源：http://hz.cheryme.top/gtuvglxlag.html

[Q73] 查看表状态
来源：http://hz.dashuyun.cn/gtlnlgooqb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.c1oappe.top/gtlxqgzoca.html

[Q74] 强制使用索引
来源：http://hz.hongshengwenyu.top/gtnrnvaafd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.xylfe.cn/gtxgsewlor.html

[Q75] 日期格式化
来源：http://hz.jinghuilouyu.cn/gtkeldptnc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.havefunace.top/gtmkghvtkw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.zhiwuduotai.top/gtcymwuknl.html

[Q76] 按天统计
来源：http://hz.daria6918.cn/gtyedunfqz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.nanxuanxn.top/gtkdocakef.html

[Q77] 时间加减
来源：http://hz.yuxming.cn/gthahczqha.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hysaishi.cn/gtypmksrih.html

[Q78] 当前时间
来源：http://hz.hnxiangtu.top/gtyvqwznin.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.kuanghao11.cn/gtysetbhxb.html

[Q79] 字符串拼接
来源：http://hz.meibo888.top/gtndtkiuyw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.haohaochexian.top/gtiwpargwo.html

[Q80] 字符串截取
来源：http://hz.cashguo.top/gtoqkmzpyy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yongpay.top/gtgicxjato.html

[Q81] 字符串替换
来源：http://hz.jinyuanbaomall.cn/gtegfwjtyf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.yueranfly.top/gtcfmxyqrx.html

[Q82] 字符长度与字节长度
来源：http://hz.aibaodan.cn/gturjklctr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtuoawxaey.html

[Q83] 大小写转换
来源：http://hz.gogol.net.cn/gtdqihtses.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.gotoacloud.top/gtnubgyukk.html

[Q84] 去除首尾空格
来源：http://hz.gzhubu.top/gtcamvvfjf.html

SELECT TRIM(name) FROM users;
来源：http://hz.yangfankeji.com/gtbamwfssp.html

[Q85] 数值取整
来源：http://hz.gogol.net.cn/gtucdwzojq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.haohaochexian.top/gtxmkhynbx.html

[Q86] 读取 JSON 字段
来源：http://hz.jyoumei.cn/gtrqefqblu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.guowangkeji.top/gtmincphlv.html

[Q87] JSON 字段做条件
来源：http://hz.xziqi.cn/gtsrdezncs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenzaomai.com/gtwcmugney.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydzc1.top/gtzvjtqgol.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.cheryme.top/gtzirtfiph.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.jqgufenzy.top/gtlqvnnkwe.html

[Q89] 判断表是否存在
来源：http://hz.jlsjyb.cn/gtstzisxqd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sxryk.cn/gtdhwohcvm.html

[Q90] 生成序号列
来源：http://hz.yanxiufei.cn/gtdzjokqkl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.zhaomingkeji.xyz/gtvgcgdmao.html

================================================================================
来源：http://hz.shangyingyoupin.top/gtfhlpsaso.html

R. Bash 专题
来源：http://hz.birdmap.top/gtyvvahqde.html

================================================================================
来源：http://hz.jinqigfzy.top/gtwjuglayb.html

[R01] shebang 与严格模式
来源：http://hz.jinqigufen.top/gtfvjztuiw.html

#!/usr/bin/env bash
来源：http://hz.pengpengdd.cyou/gtutmwdjoy.html

set -euo pipefail
来源：http://hz.zhixingplan.top/gtjhimklwd.html

[R02] 变量赋值与使用
来源：http://hz.xylfe.cn/gtdutxpual.html

name="Tom"; echo "$name"
来源：http://hz.yanxiufei.cn/gtgjvoidux.html

[R03] 只读变量
来源：http://hz.aizwys.cn/gtpsczkqma.html

readonly PI=3.14
来源：http://hz.shanyushiyangkeji.top/gtqskbfsni.html

[R04] 位置参数
来源：http://hz.zhoulong.xyz/gtxrjopenv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.yuxming.cn/gtttmdlejw.html

[R05] 参数默认值
来源：http://hz.jiagoushi.top/gtjmkluorf.html

name="${1:-default}"
来源：http://hz.zhixingplan.top/gtbbzxsfgm.html

[R06] 判断命令是否存在
来源：http://hz.svipenyu.cn/gtzqqmetbd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.hammf.cn/gtbalsafty.html

[R07] if 判断文件
来源：http://hz.wangshuangyany.cn/gtzogjpdpv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.jianghu66.top/gtugfuntlu.html

[R08] 数值比较
来源：http://hz.ydzc1.top/gtfgrjdgms.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.mhx1999.top/gtwzpclpvi.html

[R09] 字符串比较
来源：http://hz.sxryk.cn/gtmktwtilt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.pengpengdd.cyou/gtpqcbxzwd.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtqlnfdfpp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.sufxvd.cn/gtgxfifjxw.html

[R11] case 多分支
来源：http://hz.chenzaomai.com/gtgjyeejmt.html

case "$1" in
来源：http://hz.hnqzz.top/gtzsabzuix.html

start) echo "启动" ;;
来源：http://hz.sufxvd.cn/gtnmeiophj.html

stop)  echo "停止" ;;
来源：http://hz.mhx1999.top/gtplzjqymd.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtdvbpuerh.html

esac
来源：http://hz.sysykeji.top/gtcpgiirem.html

[R12] for 遍历文件
来源：http://hz.nanxinkj.top/gtobwllxjf.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shangyingyoupin.top/gtrcftbnnb.html

[R13] for 计数循环
来源：http://hz.gaohongyu789.top/gtyqdjokcq.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.yuanzhike.top/gtpldvmrun.html

[R14] C 风格 for
来源：http://hz.hongshengwenyu.top/gtbomrfzar.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xuanzx.com/gtfiluzasc.html

[R15] while 逐行读文件
来源：http://hz.gotoacloud.top/gtomtbjvmb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.andypj.xyz/gtjadcknyx.html

[R16] until 等待条件
来源：http://hz.xingfuxueyuan.xyz/gtxmauypfi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.bjfxy.top/gtpkjbnzdj.html

[R17] 数组定义与取值
来源：http://hz.yj20258.top/gtyhksdpxm.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yuanzhike.top/gtvxyjikqx.html

[R18] 遍历数组
来源：http://hz.shanyushiyangtech.top/gtzzgxlfze.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhixingplan.top/gtdloljjsc.html

[R19] 数组长度
来源：http://hz.chenzaomai.com/gtjtnqyxck.html

echo "${#arr[@]}"
来源：http://hz.sxryk.cn/gtzcdrrfas.html

[R20] 关联数组（字典）
来源：http://hz.daria6918.cn/gtvgmpxzdj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.iojbl.cn/gtmvoljsbk.html

[R21] 字符串长度
来源：http://hz.redwolf501.top/gtczlmbcbi.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gthgpzuvkt.html

[R22] 截取子串
来源：http://hz.wangshuangyany.cn/gttcmdjwpr.html

echo "${s:0:5}"
来源：http://hz.c1oappe.top/gtmfefasqm.html

[R23] 字符串替换
来源：http://hz.guannengcc.top/gtvgyvkcws.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.zdqjudy.top/gttkpfvfwo.html

[R24] 大小写转换
来源：http://hz.jinqigfzy.top/gtsmkjqkaz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.fengsongda.top/gtscczcjui.html

[R25] 去后缀 / 去前缀
来源：http://hz.ydjk.org.cn/gtwueorkvx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.zhijiandao.cn/gtotcdtebs.html

[R26] 命令替换
来源：http://hz.316326.xyz/gtyjpcwzck.html

now=$(date +%F); echo "$now"
来源：http://hz.zhengqikj.top/gthkgieeje.html

[R27] 算术展开
来源：http://hz.ydzc1.top/gtvyzcsbwx.html

echo $((1 + 2 * 3))
来源：http://hz.wangdashe.top/gtgezougzv.html

[R28] 浮点运算
来源：http://hz.tanke756.top/gtwxumzsvu.html

echo "scale=2; 10/3" | bc
来源：http://hz.nwbrower.top/gtfqbyfmag.html

[R29] 定义函数
来源：http://hz.hysaishi.cn/gtuqxndldj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.yj202588.top/gtodbvgsar.html

[R30] 函数返回状态码
来源：http://hz.redwolf501.top/gtfvznbygp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.pycfn.com/gthoxarcja.html

[R31] 局部变量
来源：http://hz.jyoumei.cn/gtiwdozqlx.html

f() { local x=1; echo "$x"; }
来源：http://hz.kuanghao11.cn/gtylwxmgsv.html

[R32] 参数个数校验
来源：http://hz.jinqigufen.top/gtwlrgyfnp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.fzhhl.top/gtbetkbdnv.html

[R33] 捕获错误并提示行号
来源：http://hz.9152youxi.cn/gtjsxcmhoh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.wangdashe.top/gtonxtsowx.html

[R34] 退出时清理
来源：http://hz.ppjwa.cn/gtwqgiqwcq.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtbvbbapfw.html

[R35] 后台执行并等待
来源：http://hz.xingfuxueyuan.xyz/gtsocnjsjo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenzaomai.com/gthjbzzznp.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gtnvrsoprd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.snrcjt.cn/gtyomlcidr.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtcwstuxho.html

files=$(ls -1)
来源：http://hz.52xcode.cn/gtfwjeprmo.html

[R38] 管道串联
来源：http://hz.iojbl.cn/gtpsdpnwfe.html

cat a.txt | grep -i error | wc -l
来源：http://hz.tianlin.xyz/gtbtaswlca.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtkfvkbdpf.html

cmd > out.log 2>&1
来源：http://hz.zycfv.cn/gtxhtqxspl.html

[R40] 追加写日志
来源：http://hz.xingfuxueyuan.xyz/gtqambaqxj.html

echo "log" >> out.log
来源：http://hz.fzhhl.top/gtiictgrhg.html

[R41] 丢弃输出
来源：http://hz.hammf.cn/gtzbqdumlx.html

cmd >/dev/null 2>&1
来源：http://hz.jqgufenzy.top/gttnxalexr.html

[R42] 输入重定向
来源：http://hz.havefunace.top/gtxltutvwa.html

wc -l < a.txt
来源：http://hz.c1oappe.top/gtcmdygezc.html

[R43] 按名字查找文件
来源：http://hz.havefunace.top/gtdzckdqzh.html

find . -name "*.log" -type f
来源：http://hz.vqdsnc.cn/gtjisuqmfr.html

[R44] 按修改时间查找
来源：http://hz.xziqi.cn/gtyupowoip.html

find . -mtime -7 -type f
来源：http://hz.feifeiyinyue.top/gtijxdheob.html

[R45] 批量删除
来源：http://hz.jinyuanbaomall.cn/gtflkytxkp.html

find . -name "*.tmp" -delete
来源：http://hz.cucudq.cn/gtufpopasn.html

[R46] 递归替换文件内容
来源：http://hz.shuidangran.top/gtpwattygy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.dashuyun.cn/gtktsfmknf.html

[R47] sed 单行替换
来源：http://hz.xziqi.cn/gtghqhjrhf.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.chenzaomai.com/gtqmglhqvu.html

[R48] awk 取指定列
来源：http://hz.aizwys.cn/gtcekbtxig.html

awk '{print $1, $3}' a.txt
来源：http://hz.hnqzz.top/gtsilvluoc.html

[R49] awk 带条件
来源：http://hz.jianghu66.top/gtmayicuci.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.c1oappe.top/gtntbtgqmd.html

[R50] awk 求和
来源：http://hz.cucudq.cn/gttmnckbkg.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jinyuanbaomall.cn/gtwcwfrtal.html

[R51] 排序去重取前几
来源：http://hz.jinghuilouyu.cn/gtobjawbei.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.sweek.top/gtuztfefmh.html

[R52] 统计行数
来源：http://hz.tian-w.cn/gtqlydwyug.html

wc -l a.txt
来源：http://hz.gzhubu.top/gtmgxnshla.html

[R53] 查看文件头与实时尾
来源：http://hz.yanxiufei.cn/gtckmbupmj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.ybcxt.top/gthyrrcxfq.html

[R54] 比较两个文件
来源：http://hz.zycfv.cn/gtssjkaqbj.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtdptmjaic.html

[R55] 压缩与解压
来源：http://hz.52xcode.cn/gtwyzyggqp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhoulong.xyz/gtlqsnizcz.html

[R56] 远程拷贝
来源：http://hz.zhijiandao.cn/gtnonkbcjm.html

scp file user@host:/path/
来源：http://hz.zhijiandao.cn/gtcezbxtda.html

[R57] 远程执行命令
来源：http://hz.xingfuxueyuan.xyz/gtcatzvjib.html

ssh user@host 'uptime'
来源：http://hz.svipenyu.cn/gthcsxrgsx.html

[R58] 下载文件
来源：http://hz.zhijiandao.cn/gtbubtaybf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.jyoumei.cn/gtslrmpdhd.html

[R59] 发 POST JSON
来源：http://hz.kuanghao11.cn/gtvezdfjwb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.hfpthk.cn/gtylkhdxkp.html

[R60] 只看 HTTP 状态码
来源：http://hz.fzhhl.top/gtotjupnnt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yj202588.top/gtfoyktiwf.html

[R61] 磁盘占用
来源：http://hz.9152youxi.cn/gtzxotohxb.html

df -h;  du -sh *
来源：http://hz.xingfuxueyuan.xyz/gtljecntno.html

[R62] 找最占空间的文件
来源：http://hz.xylfe.cn/gtuxlvxinx.html

du -ah . | sort -rh | head -10
来源：http://hz.xinyue.icu/gtertxuqeq.html

[R63] 内存与进程
来源：http://hz.gaohongyu789.top/gtwrprgivs.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtltoxbzzd.html

[R64] 结束进程
来源：http://hz.jyoumei.cn/gtzqamjgfi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.guannengcc.top/gtncgwzcfp.html

[R65] 查看端口占用
来源：http://hz.dianchejie.cn/gtifqymexh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.aibaodan.cn/gtrcdnxzel.html

[R66] 定时任务
来源：http://hz.sxryk.cn/gtvzceuqkj.html

crontab -e;  crontab -l
来源：http://hz.jinyuanbaomall.cn/gtdgtdjacu.html

[R67] 生成随机十六进制串
来源：http://hz.daxiang520.top/gtrigjtalk.html

openssl rand -hex 16
来源：http://hz.sysykeji.top/gtdsxkagce.html

[R68] 计算文件校验值
来源：http://hz.pengpengdd.cyou/gtbwmgztco.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.hammf.cn/gtjpntgvwc.html

[R69] 生成随机密码
来源：http://hz.sysykeji.top/gtyswcbwmx.html

head -c 16 /dev/urandom | base64
来源：http://hz.andypj.xyz/gtmdkhyegf.html

[R70] 时间戳与互转
来源：http://hz.yueranfly.top/gtbabahbak.html

date +%s;  date -d @1700000000
来源：http://hz.aibaodan.cn/gtlasnqjth.html

[R71] 日期格式化
来源：http://hz.yvedp.cn/gtlrieswug.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.tian-w.cn/gthxszittp.html

[R72] 等待端口就绪
来源：http://hz.jlsjyb.cn/gtyeqqozok.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sufxvd.cn/gteblthaxe.html

[R73] 分割大日志
来源：http://hz.zhaomingkeji.xyz/gtvhttehyz.html

split -l 1000 big.log part_
来源：http://hz.hongshengwenyu.top/gtlilqifzx.html

[R74] 批量重命名
来源：http://hz.shuidangran.top/gtlbjwldxo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.yj202588.top/gtjgmrkffs.html

[R75] 导出环境变量
来源：http://hz.haohaochexian.top/gtpoztlyoq.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.0kj1m.cn/gtlywjonja.html

[R76] 使用临时文件
来源：http://hz.0kj1m.cn/gtobepsqgi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.gzhubu.top/gtemyxzcyd.html

[R77] 读取用户输入
来源：http://hz.yuanzhike.top/gtwnijnfbr.html

read -rp "请输入: " ans
来源：http://hz.zhengqikj.top/gtedzeheav.html

[R78] 交互式菜单
来源：http://hz.smart0.xyz/gtogedxxxg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.nwbrower.top/gtezwovhji.html

[R79] 解析命令行选项
来源：http://hz.feifeiyinyue.top/gthnmtfexa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.cqqwz.cn/gtchjcfbjs.html

[R80] 查看脚本执行耗时
来源：http://hz.xingfuxueyuan.xyz/gthaducexy.html

time ./run.sh
来源：http://hz.guannengcc.top/gtdngglqjf.html

================================================================================
来源：http://hz.ydzc1.top/gthbgslauv.html

S. C / C++ 专题
来源：http://hz.yanxiufei.cn/gtxfvlloui.html

================================================================================
来源：http://hz.svipenyu.cn/gtzklvwhxw.html

[S01] C：Hello World
来源：http://hz.ehwqpu.com/gtluymutlo.html

#include <stdio.h>
来源：http://hz.ehwqpu.com/gtqsnpmzbm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.xziqi.cn/gtptyehiab.html

[S02] C：变量与格式化输出
来源：http://hz.jyoumei.cn/gtteizbgrq.html

int a = 10; printf("%d\n", a);
来源：http://hz.sysykeji.top/gtebbkwojz.html

[S03] C：读入整数
来源：http://hz.ydzc1.top/gtjypsgger.html

int x; scanf("%d", &x);
来源：http://hz.zhiwuduotai.top/gttjrullqr.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtejxwwawm.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.jyoumei.cn/gtovdbflog.html

[S05] C：字符串长度
来源：http://hz.guowangkeji.top/gtwhtvmqvx.html

strlen(s)
来源：http://hz.tianlin.xyz/gttfvvbnon.html

[S06] C：字符串比较
来源：http://hz.ybcxt.top/gtnluwcbdh.html

strcmp(a, b) == 0
来源：http://hz.chenjidiqi.icu/gtjwrhwsjc.html

[S07] C：数组遍历求和
来源：http://hz.xinyue.icu/gtmehgqnql.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xuanzx.com/gtcjvhbtkb.html

[S08] C：动态内存分配与释放
来源：http://hz.hfpthk.cn/gtwugkqnjn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yangfankeji.com/gtfmyaguli.html

[S09] C：结构体定义与初始化
来源：http://hz.meibo888.top/gttdmssxbr.html


<!-- 参考信息 -->