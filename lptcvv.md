代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://hz.zhaomingkeji.xyz/gtkebjmbfy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://hz.jinqigfzy.top/gtdgwxwnuv.html

[Q39] 自连接（查上下级）
来源：http://hz.hammf.cn/gtpcruowef.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://hz.cdnleiting.top/gtkiqbksox.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://hz.ywan-chungtsiang.top/gtayysoniy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://hz.hywenlv.cn/gtlyrqngrc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://hz.hywenlv.cn/gtbddznhij.html

[Q41] 多表连接
来源：http://hz.daria6918.cn/gtigygxwyi.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://hz.dashuyun.cn/gteysvqdhc.html

JOIN users u ON u.id = o.user_id
来源：http://hz.yuanzhike.top/gtommzjokk.html

JOIN products p ON p.id = o.product_id;
来源：http://hz.xuetiantiany.cn/gtcfgqnuov.html

[Q42] 连接条件附加过滤
来源：http://hz.xylfe.cn/gtwvegzomq.html

SELECT u.name, o.amount FROM users u
来源：http://hz.aizwys.cn/gtweenoujf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://hz.bjfxy.top/gtfsmlnrbv.html

[Q43] 标量子查询
来源：http://hz.shuidangran.top/gtmdwdiakb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://hz.nwbrower.top/gthjjxpmxc.html

[Q44] IN 子查询
来源：http://hz.gogol.net.cn/gtfrquyfjs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://hz.jiagoushi.top/gtysjkdyan.html

[Q45] EXISTS 判断存在
来源：http://hz.xingfuxueyuan.xyz/gtpidqmocl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.snrcjt.cn/gtudbqiiph.html

[Q46] NOT EXISTS 判断不存在
来源：http://hz.gzhubu.top/gtxxthsrgb.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://hz.smart0.xyz/gtyuvljgpk.html

[Q47] 与平均值比较
来源：http://hz.jqgufenzy.top/gttyuezjoe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://hz.yj20258888.top/gtmvotmyip.html

[Q48] CTE 公用表表达式
来源：http://hz.xuanzx.com/gtkmfrgchp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://hz.ivvv.top/gtfrystjla.html

SELECT * FROM t WHERE c > 5;
来源：http://hz.zhixingplan.top/gtokywfqya.html

[Q49] 更新单行
来源：http://hz.jianghu66.top/gtnqrmxsaf.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.chenzaomai.com/gtfaxqgctt.html

[Q50] 批量更新
来源：http://hz.yonumen.top/gtbzjxride.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.chenjidiqi.icu/gtquvtasqv.html

[Q51] 用子查询更新
来源：http://hz.ydzc1.top/gtyncppeim.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.jinyuanbaomall.cn/gtyhnwxwqy.html

[Q52] 删除指定行
来源：http://hz.zdqjudy.top/gtoxqkhnfq.html

DELETE FROM users WHERE id = 10;
来源：http://hz.iojbl.cn/gtsqienacp.html

[Q53] 按条件删除
来源：http://hz.yj202588.top/gtxdjdrxjj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.mhx1999.top/gtrfusykfu.html

[Q54] 清空表
来源：http://hz.chenzaomai.com/gtkjuiiqxz.html

TRUNCATE TABLE logs;
来源：http://hz.jinghuilouyu.cn/gtajkwnfvg.html

[Q55] 排名（并列占位）
来源：http://hz.yuanzhike.top/gtdzruxhdm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.shanyushiyangkeji.top/gtmscijxbt.html

[Q56] 密集排名（并列不占位）
来源：http://hz.sweek.top/gtxyjarhpw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.hywenlv.cn/gtchzifhap.html

[Q57] 行号
来源：http://hz.zhijiandao.cn/gtktwtzrot.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.yvedp.cn/gtrnvihhof.html

[Q58] 累计求和
来源：http://hz.yanxiufei.cn/gtpsxoqtvm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.gaohongyu789.top/gtprscholn.html

[Q59] 分组内累计
来源：http://hz.yongpay.top/gtpzbmlusi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.iojbl.cn/gtocnfdmms.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhongyouzk.top/gtewnygzem.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.bjfxy.top/gtnpulnuua.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.wangshuangyany.cn/gtkaelzfxl.html

[Q61] 移动平均
来源：http://hz.52xcode.cn/gtdtercvrx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.dashuyun.cn/gtuuiswtps.html

[Q62] 分组占比
来源：http://hz.jyoumei.cn/gtwfjzubql.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.guannengcc.top/gtkqwiyydj.html

[Q63] 开启事务
来源：http://hz.xylfe.cn/gtfldylwzh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jinqigfzy.top/gtbfhjbnmf.html

[Q64] 提交事务
来源：http://hz.zhongyouzk.top/gtbusymrgt.html

COMMIT;
来源：http://hz.guowangkeji.top/gtmnylmoaq.html

[Q65] 回滚事务
来源：http://hz.sufxvd.cn/gtyncyhnyb.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtkolutcmf.html

[Q66] 行锁查询
来源：http://hz.jinqigufen.top/gttgdavazu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.chenjidiqi.icu/gtsmnjrrez.html

[Q67] 设置隔离级别
来源：http://hz.wangshuangyany.cn/gtqmsxxcim.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.vqdsnc.cn/gtzitqnscj.html

[Q68] 保存点
来源：http://hz.xingfuxueyuan.xyz/gtvzlenajc.html

SAVEPOINT sp1;
来源：http://hz.hongshengwenyu.top/gtawzpaekt.html

ROLLBACK TO sp1;
来源：http://hz.zdqjudy.top/gtwipqjkcg.html

[Q69] 查看执行计划
来源：http://hz.ydjk.org.cn/gtdpsssity.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.jianghu66.top/gtdshscsku.html

[Q70] 更新统计信息
来源：http://hz.jinyuanbaomall.cn/gtxcepmhjp.html

ANALYZE TABLE users;
来源：http://hz.shuidangran.top/gtivfswmic.html

[Q71] 查看建表语句
来源：http://hz.yongpay.top/gtwjmalhjb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.52xcode.cn/gtbsnodzou.html

[Q72] 查看索引
来源：http://hz.zhoulong.xyz/gtrnjkxcnd.html

SHOW INDEX FROM users;
来源：http://hz.zhoulong.xyz/gtrlzhtyxl.html

[Q73] 查看表状态
来源：http://hz.wangshuangyany.cn/gttywrmewb.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.zhijiandao.cn/gtwiphwolm.html

[Q74] 强制使用索引
来源：http://hz.52xcode.cn/gtbclcoruo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.ppjwa.cn/gtfdhdleyy.html

[Q75] 日期格式化
来源：http://hz.c1oappe.top/gtovlertai.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.xingfuxueyuan.xyz/gtpodbhvmx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yangfankeji.com/gtqxflwhpu.html

[Q76] 按天统计
来源：http://hz.hammf.cn/gtqgqxmzsm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.haohaochexian.top/gtivcihwlb.html

[Q77] 时间加减
来源：http://hz.nwbrower.top/gtrykluvjv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.chenjidiqi.icu/gtmviyhtno.html

[Q78] 当前时间
来源：http://hz.hfpthk.cn/gtlspkitkx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.cqqwz.cn/gtwezntvqg.html

[Q79] 字符串拼接
来源：http://hz.zhixingplan.top/gtxrjtadyy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.snrcjt.cn/gtvzgnvbmq.html

[Q80] 字符串截取
来源：http://hz.redwolf501.top/gtdftrxhjp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.vqdsnc.cn/gtsbqgvahh.html

[Q81] 字符串替换
来源：http://hz.cucudq.cn/gtqzkcnplj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.shzxlz.cn/gtmxgfqiiz.html

[Q82] 字符长度与字节长度
来源：http://hz.tianlin.xyz/gtjlqnqxns.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.zhaomingkeji.xyz/gtwxcexfya.html

[Q83] 大小写转换
来源：http://hz.zhengqikj.top/gtcrjpaegl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.sweek.top/gtuwjyxypn.html

[Q84] 去除首尾空格
来源：http://hz.gogol.net.cn/gtfgxkmsdg.html

SELECT TRIM(name) FROM users;
来源：http://hz.andypj.xyz/gttotoizkd.html

[Q85] 数值取整
来源：http://hz.hnqzz.top/gtebnvdpzb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.gaohongyu789.top/gtfsmizuew.html

[Q86] 读取 JSON 字段
来源：http://hz.daxiang520.top/gttcamypcv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.52xcode.cn/gtrwmlbafl.html

[Q87] JSON 字段做条件
来源：http://hz.ywan-chungtsiang.top/gtbinktxic.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.smart0.xyz/gthvayenrq.html

[Q88] 行转列（条件聚合）
来源：http://hz.zhiwuduotai.top/gtjxyrvgpq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.ivvv.top/gtipromocv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hammf.cn/gtnjonxzie.html

[Q89] 判断表是否存在
来源：http://hz.vqdsnc.cn/gtmersicsk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.andypj.xyz/gtnrvwrbda.html

[Q90] 生成序号列
来源：http://hz.hammf.cn/gtlihtfbjr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.vqdsnc.cn/gtfkuxgmrd.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtrbistumn.html

R. Bash 专题
来源：http://hz.vqdsnc.cn/gtbnensnor.html

================================================================================
来源：http://hz.gaohongyu789.top/gtbsdxscvs.html

[R01] shebang 与严格模式
来源：http://hz.bjfxy.top/gtbzrjufxd.html

#!/usr/bin/env bash
来源：http://hz.ywan-chungtsiang.top/gtdbqabxjy.html

set -euo pipefail
来源：http://hz.sysykeji.top/gtapmxhugb.html

[R02] 变量赋值与使用
来源：http://hz.jinyuanbaomall.cn/gtpufabonh.html

name="Tom"; echo "$name"
来源：http://hz.ydjk.org.cn/gtmfkhxmsl.html

[R03] 只读变量
来源：http://hz.guowangkeji.top/gtcklacguj.html

readonly PI=3.14
来源：http://hz.jqgfzy.top/gthjzdfiec.html

[R04] 位置参数
来源：http://hz.0kj1m.cn/gtofjrbisy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.ywan-chungtsiang.top/gtfthffzuz.html

[R05] 参数默认值
来源：http://hz.yj20258888.top/gtrzbwnfnd.html

name="${1:-default}"
来源：http://hz.hfpthk.cn/gtdfikwrpb.html

[R06] 判断命令是否存在
来源：http://hz.wangdashe.top/gtdebmlpzz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.gogol.net.cn/gtxecrvnnw.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtxnadsyzo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.havefunace.top/gtqosgveoz.html

[R08] 数值比较
来源：http://hz.hywenlv.cn/gtfpnlfkyy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.zhijiandao.cn/gtxkadwtvy.html

[R09] 字符串比较
来源：http://hz.xylfe.cn/gtunbhqtpv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.sufxvd.cn/gtdzgvlkij.html

[R10] 正则匹配
来源：http://hz.yangfankeji.com/gtynctlbqz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.316326.xyz/gtvlkimeei.html

[R11] case 多分支
来源：http://hz.nanxinkj.top/gtxdzjeihn.html

case "$1" in
来源：http://hz.chenlongwang.top/gtdzgiaspx.html

start) echo "启动" ;;
来源：http://hz.jlsjyb.cn/gtfzvihxpe.html

stop)  echo "停止" ;;
来源：http://hz.yuxming.cn/gtlngjpvfg.html

*)     echo "未知命令" ;;
来源：http://hz.gotoacloud.top/gtpzakbbtv.html

esac
来源：http://hz.jinghuilouyu.cn/gtqkmqfxkn.html

[R12] for 遍历文件
来源：http://hz.c1oappe.top/gtetvtcazh.html

for f in *.txt; do echo "$f"; done
来源：http://hz.zhongyouzk.top/gtahfgmulp.html

[R13] for 计数循环
来源：http://hz.yongpay.top/gtcmfpkcsk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.316326.xyz/gtziybbxfi.html

[R14] C 风格 for
来源：http://hz.cashguo.top/gtizxehdxm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.zhengqikj.top/gtxgcenyye.html

[R15] while 逐行读文件
来源：http://hz.hysaishi.cn/gtkyyfegcc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.jqgfzy.top/gtvemvlhnb.html

[R16] until 等待条件
来源：http://hz.wangdashe.top/gtkhprfmfy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.havefunace.top/gtnbomukhv.html

[R17] 数组定义与取值
来源：http://hz.yueranfly.top/gtppofhyki.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yueranfly.top/gtruhkkkop.html

[R18] 遍历数组
来源：http://hz.0kj1m.cn/gtdlpktbvo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.xinyue.icu/gtwgiymhlo.html

[R19] 数组长度
来源：http://hz.yanxiufei.cn/gttnvrtvkd.html

echo "${#arr[@]}"
来源：http://hz.hammf.cn/gtjgpxpcct.html

[R20] 关联数组（字典）
来源：http://hz.shanyushiyangkeji.top/gtnfmfswwh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.shzxlz.cn/gtytqinygr.html

[R21] 字符串长度
来源：http://hz.kuanghao11.cn/gtsudmdxdd.html

echo "${#s}"
来源：http://hz.jinghuilouyu.cn/gtjllpsbeg.html

[R22] 截取子串
来源：http://hz.hongshengwenyu.top/gtugehwsib.html

echo "${s:0:5}"
来源：http://hz.snrcjt.cn/gtyjuyfgoh.html

[R23] 字符串替换
来源：http://hz.nanxuanxn.top/gtkurszbrr.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.vqdsnc.cn/gtvlfxobol.html

[R24] 大小写转换
来源：http://hz.yanxiufei.cn/gtigruautw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.zhixingplan.top/gtssmmlfkc.html

[R25] 去后缀 / 去前缀
来源：http://hz.dashuyun.cn/gtikxzqitb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.aibaodan.cn/gtcyudvopq.html

[R26] 命令替换
来源：http://hz.jianghu66.top/gtsixfcvlt.html

now=$(date +%F); echo "$now"
来源：http://hz.xinyue.icu/gtcivyticn.html

[R27] 算术展开
来源：http://hz.xuetiantiany.cn/gtxagkxesd.html

echo $((1 + 2 * 3))
来源：http://hz.smart0.xyz/gtyqucnjwi.html

[R28] 浮点运算
来源：http://hz.redwolf501.top/gtaqqzyome.html

echo "scale=2; 10/3" | bc
来源：http://hz.mhx1999.top/gtlzhnaptq.html

[R29] 定义函数
来源：http://hz.xinyue.icu/gtiwbphbbd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.xuanzx.com/gtxoyqsrju.html

[R30] 函数返回状态码
来源：http://hz.hammf.cn/gtoulitjyy.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.yj20258.top/gtlhoamjww.html

[R31] 局部变量
来源：http://hz.52xcode.cn/gtveyebguv.html

f() { local x=1; echo "$x"; }
来源：http://hz.yueranfly.top/gtmvrlpphc.html

[R32] 参数个数校验
来源：http://hz.havefunace.top/gtysxdraop.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.chenzaomai.com/gtqjmnkgbo.html

[R33] 捕获错误并提示行号
来源：http://hz.cashguo.top/gthwefkhdq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtakkhxbyx.html

[R34] 退出时清理
来源：http://hz.jiagoushi.top/gtvxplfaze.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.gaohongyu789.top/gtqedjjgxx.html

[R35] 后台执行并等待
来源：http://hz.nanxinkj.top/gtjkfwfcec.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.andypj.xyz/gtzoawujwm.html

[R36] 并发执行多个任务
来源：http://hz.ydjk.org.cn/gtqcwshbgc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cqqwz.cn/gtxaenvetk.html

[R37] 把输出赋给变量
来源：http://hz.aizwys.cn/gtxnvbqsxn.html

files=$(ls -1)
来源：http://hz.cashguo.top/gtcgahupvp.html

[R38] 管道串联
来源：http://hz.hywenlv.cn/gttchykyea.html

cat a.txt | grep -i error | wc -l
来源：http://hz.mhx1999.top/gtchzdbnha.html

[R39] 重定向标准输出与错误
来源：http://hz.feifeiyinyue.top/gtsuzvclut.html

cmd > out.log 2>&1
来源：http://hz.chenlongwang.top/gtnfaqxrku.html

[R40] 追加写日志
来源：http://hz.svipenyu.cn/gtttpumyiu.html

echo "log" >> out.log
来源：http://hz.yj20258888.top/gtjtjfnikj.html

[R41] 丢弃输出
来源：http://hz.sufxvd.cn/gtgnrgmjvb.html

cmd >/dev/null 2>&1
来源：http://hz.cdnleiting.top/gtcgpugxei.html

[R42] 输入重定向
来源：http://hz.hnqzz.top/gtopdypopa.html

wc -l < a.txt
来源：http://hz.gotoacloud.top/gtkrdgbnyp.html

[R43] 按名字查找文件
来源：http://hz.xingfuxueyuan.xyz/gtkraeqsyf.html

find . -name "*.log" -type f
来源：http://hz.dashuyun.cn/gtnsusvght.html

[R44] 按修改时间查找
来源：http://hz.smart0.xyz/gtefrcjkvg.html

find . -mtime -7 -type f
来源：http://hz.gzhubu.top/gtematpakc.html

[R45] 批量删除
来源：http://hz.ydjk.org.cn/gtwgeiytcd.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258.top/gtnuyskrxd.html

[R46] 递归替换文件内容
来源：http://hz.yueranfly.top/gtgrquuhfg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.yonumen.top/gtkpnjaoub.html

[R47] sed 单行替换
来源：http://hz.vqdsnc.cn/gtkayduafj.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.ywan-chungtsiang.top/gtxidtjkjw.html

[R48] awk 取指定列
来源：http://hz.vqdsnc.cn/gtlwidvbwd.html

awk '{print $1, $3}' a.txt
来源：http://hz.jqgfzy.top/gtgogaaodl.html

[R49] awk 带条件
来源：http://hz.gaohongyu789.top/gtaihkxcal.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.guowangkeji.top/gtyiywbazv.html

[R50] awk 求和
来源：http://hz.9152youxi.cn/gtoptkipjx.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.jianghu66.top/gtvgmpitxy.html

[R51] 排序去重取前几
来源：http://hz.zhijiandao.cn/gtpsrnjpwr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.ywan-chungtsiang.top/gttgvlamxz.html

[R52] 统计行数
来源：http://hz.shuidangran.top/gtstvumhsc.html

wc -l a.txt
来源：http://hz.xinyue.icu/gtwvqqoqzd.html

[R53] 查看文件头与实时尾
来源：http://hz.zycfv.cn/gtofayurfg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hywenlv.cn/gtxfkprvje.html

[R54] 比较两个文件
来源：http://hz.yvedp.cn/gtayheaukh.html

diff a.txt b.txt
来源：http://hz.sysykeji.top/gtktjcstaw.html

[R55] 压缩与解压
来源：http://hz.svipenyu.cn/gtkfdmdtqz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.smart0.xyz/gtpzartpgr.html

[R56] 远程拷贝
来源：http://hz.zhongyouzk.top/gtwerzdixn.html

scp file user@host:/path/
来源：http://hz.vqdsnc.cn/gtjdxccyys.html

[R57] 远程执行命令
来源：http://hz.cucudq.cn/gtqkugmwaf.html

ssh user@host 'uptime'
来源：http://hz.zhoulong.xyz/gtkjdmwjvg.html

[R58] 下载文件
来源：http://hz.chenzaomai.com/gttsphnrbz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.iojbl.cn/gtbqyuwxbq.html

[R59] 发 POST JSON
来源：http://hz.zhongyouzk.top/gtbnmwjspe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.aibaodan.cn/gtivcyyqgf.html

[R60] 只看 HTTP 状态码
来源：http://hz.zhiwuduotai.top/gtxxercxdc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.yvedp.cn/gtuxtyqcpb.html

[R61] 磁盘占用
来源：http://hz.snrcjt.cn/gtuueivvmv.html

df -h;  du -sh *
来源：http://hz.52xcode.cn/gtudclcqii.html

[R62] 找最占空间的文件
来源：http://hz.9152youxi.cn/gtsswjceqx.html

du -ah . | sort -rh | head -10
来源：http://hz.feifeiyinyue.top/gtgyknsgtl.html

[R63] 内存与进程
来源：http://hz.sxryk.cn/gtuwunvrtu.html

free -h;  ps aux | grep nginx
来源：http://hz.pycfn.com/gtfevtpbbm.html

[R64] 结束进程
来源：http://hz.nanxuanxn.top/gttwjuavai.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yuxming.cn/gtwzildhho.html

[R65] 查看端口占用
来源：http://hz.zhongyouzk.top/gtlruozhdx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.redwolf501.top/gtytjiwmpm.html

[R66] 定时任务
来源：http://hz.xylfe.cn/gtazhaedkq.html

crontab -e;  crontab -l
来源：http://hz.havefunace.top/gtewfpinfs.html

[R67] 生成随机十六进制串
来源：http://hz.ydzc1.top/gtnejsttrx.html

openssl rand -hex 16
来源：http://hz.fengsongda.top/gtvfclgpky.html

[R68] 计算文件校验值
来源：http://hz.9152youxi.cn/gtsjvmjkew.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.zhoulong.xyz/gtyzyqheaa.html

[R69] 生成随机密码
来源：http://hz.ydjk.org.cn/gtvbyccrpu.html

head -c 16 /dev/urandom | base64
来源：http://hz.aibaodan.cn/gtennamxqw.html

[R70] 时间戳与互转
来源：http://hz.wangdashe.top/gtzsmvpctt.html

date +%s;  date -d @1700000000
来源：http://hz.feifeiyinyue.top/gtzfsakqhf.html

[R71] 日期格式化
来源：http://hz.zhengqikj.top/gtebyeuwfn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.xuetiantiany.cn/gtxezwjhjk.html

[R72] 等待端口就绪
来源：http://hz.guannengcc.top/gtwcvbtekd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.nwbrower.top/gtqgoxwyjy.html

[R73] 分割大日志
来源：http://hz.yj20258888.top/gtpmuhekwr.html

split -l 1000 big.log part_
来源：http://hz.wangdashe.top/gtqosvflgr.html

[R74] 批量重命名
来源：http://hz.svipenyu.cn/gtesytcvyo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.jinghuilouyu.cn/gtadoyylck.html

[R75] 导出环境变量
来源：http://hz.gaohongyu789.top/gtkmjeqtbj.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.jinqigfzy.top/gtlcfdhqlb.html

[R76] 使用临时文件
来源：http://hz.xziqi.cn/gtifsfjrqe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xylfe.cn/gtcfxikxik.html

[R77] 读取用户输入
来源：http://hz.xylfe.cn/gtdnywuazd.html

read -rp "请输入: " ans
来源：http://hz.52xcode.cn/gthelydqkg.html

[R78] 交互式菜单
来源：http://hz.shuidangran.top/gtrxgzqlts.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jianghu66.top/gtguntakni.html

[R79] 解析命令行选项
来源：http://hz.jinqigfzy.top/gtufporztt.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.wangshuangyany.cn/gtudzcfiuw.html

[R80] 查看脚本执行耗时
来源：http://hz.jinyuanbaomall.cn/gtyntnzmnx.html

time ./run.sh
来源：http://hz.gzhubu.top/gtknusomze.html

================================================================================
来源：http://hz.aizwys.cn/gtzxrkkidc.html

S. C / C++ 专题
来源：http://hz.yj20258888.top/gtorpuvoft.html

================================================================================
来源：http://hz.gogol.net.cn/gthbqlrhii.html

[S01] C：Hello World
来源：http://hz.zhongyouzk.top/gtohqwumbi.html

#include <stdio.h>
来源：http://hz.0kj1m.cn/gttciqwsmj.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.yj20258888.top/gtshgrguzx.html

[S02] C：变量与格式化输出
来源：http://hz.hywenlv.cn/gtpgwxrbfd.html

int a = 10; printf("%d\n", a);
来源：http://hz.snrcjt.cn/gtqajgdwyc.html

[S03] C：读入整数
来源：http://hz.zdqjudy.top/gtuydocjpc.html

int x; scanf("%d", &x);
来源：http://hz.cdnleiting.top/gtbgwekdis.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtinsxhllk.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hnxiangtu.top/gtpfowvovp.html

[S05] C：字符串长度
来源：http://hz.chenzaomai.com/gtitvvhbrj.html

strlen(s)
来源：http://hz.chenlongwang.top/gtkklmvack.html

[S06] C：字符串比较
来源：http://hz.shzxlz.cn/gtewwzqkav.html

strcmp(a, b) == 0
来源：http://hz.vqdsnc.cn/gtjbarkxyc.html

[S07] C：数组遍历求和
来源：http://hz.pycfn.com/gtrnndwopr.html


<!-- 参考信息 -->