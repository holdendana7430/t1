代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://hz.shuidangran.top/gtrqvpnfki.html

[Q50] 批量更新
来源：http://hz.feifeiyinyue.top/gtrmgilgkk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://hz.yonumen.top/gtovjdlxcq.html

[Q51] 用子查询更新
来源：http://hz.chenlongwang.top/gtfdamzmzz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://hz.zhoulong.xyz/gtabghoxah.html

[Q52] 删除指定行
来源：http://hz.zhaomingkeji.xyz/gtbvexnseu.html

DELETE FROM users WHERE id = 10;
来源：http://hz.nwbrower.top/gtpqbvtbvd.html

[Q53] 按条件删除
来源：http://hz.hnqzz.top/gtocyjjpns.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://hz.svipenyu.cn/gtpqjdrzer.html

[Q54] 清空表
来源：http://hz.cdnleiting.top/gteefyobtl.html

TRUNCATE TABLE logs;
来源：http://hz.chenjidiqi.icu/gtmihbtsdv.html

[Q55] 排名（并列占位）
来源：http://hz.nwbrower.top/gtycvwpljv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://hz.jianghu66.top/gtaostwerl.html

[Q56] 密集排名（并列不占位）
来源：http://hz.hfpthk.cn/gtgsmrejsw.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://hz.xylfe.cn/gtxvrnovek.html

[Q57] 行号
来源：http://hz.zhengqikj.top/gtmdyfiado.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.svipenyu.cn/gtpxqadnix.html

[Q58] 累计求和
来源：http://hz.gotoacloud.top/gtbjyyjqmh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.nanxinkj.top/gtcsoeunew.html

[Q59] 分组内累计
来源：http://hz.feifeiyinyue.top/gtxqxolgjx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.svipenyu.cn/gtbtkxczxt.html

[Q60] 取上一行 / 下一行
来源：http://hz.aibaodan.cn/gtqwaulwvs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.yongpay.top/gtvapyofom.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.fengsongda.top/gtyilyjbpl.html

[Q61] 移动平均
来源：http://hz.tianlin.xyz/gtxxjmiaic.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.svipenyu.cn/gtwplbdyyb.html

[Q62] 分组占比
来源：http://hz.yuanzhike.top/gtpuqgwedl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.ppjwa.cn/gtsymqdzgm.html

[Q63] 开启事务
来源：http://hz.chenzaomai.com/gtapmlngpk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.zhoulong.xyz/gtyctudvku.html

[Q64] 提交事务
来源：http://hz.andypj.xyz/gtgiybbolr.html

COMMIT;
来源：http://hz.zhiwuduotai.top/gtmttpejts.html

[Q65] 回滚事务
来源：http://hz.jinghuilouyu.cn/gtrfzoywec.html

ROLLBACK;
来源：http://hz.smart0.xyz/gtfdaprkyw.html

[Q66] 行锁查询
来源：http://hz.redwolf501.top/gtbfopisqk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.gzhubu.top/gtbzjwwgjs.html

[Q67] 设置隔离级别
来源：http://hz.jlsjyb.cn/gtmekiewqy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yuxming.cn/gtgtqzocrc.html

[Q68] 保存点
来源：http://hz.yj202588.top/gtumaysrmm.html

SAVEPOINT sp1;
来源：http://hz.mhx1999.top/gtvkpkstbk.html

ROLLBACK TO sp1;
来源：http://hz.52xcode.cn/gtasgmkjru.html

[Q69] 查看执行计划
来源：http://hz.yueranfly.top/gtqjqwgdbw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.cucudq.cn/gtdzkfyqkg.html

[Q70] 更新统计信息
来源：http://hz.kuanghao11.cn/gtzuxryqqk.html

ANALYZE TABLE users;
来源：http://hz.hfpthk.cn/gtcnjguiae.html

[Q71] 查看建表语句
来源：http://hz.meibo888.top/gtsvawvsks.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zhoulong.xyz/gtpawegnsr.html

[Q72] 查看索引
来源：http://hz.daria6918.cn/gtwxflptpc.html

SHOW INDEX FROM users;
来源：http://hz.aibaodan.cn/gtsdctpazo.html

[Q73] 查看表状态
来源：http://hz.xuanzx.com/gtslxtaxji.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.smart0.xyz/gtpnqderkz.html

[Q74] 强制使用索引
来源：http://hz.xingfuxueyuan.xyz/gtvfsztdyx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.tanke756.top/gtcixnepoz.html

[Q75] 日期格式化
来源：http://hz.xylfe.cn/gtsobmgcxa.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.guannengcc.top/gtmywetpwb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.vqdsnc.cn/gtbmmmvbpp.html

[Q76] 按天统计
来源：http://hz.xuanzx.com/gtbmktngjl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.daxiang520.top/gtbknbepic.html

[Q77] 时间加减
来源：http://hz.meibo888.top/gtibogxwrv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.hongshengwenyu.top/gtocnvypay.html

[Q78] 当前时间
来源：http://hz.quarkkingdee.top/gtsolsbead.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.gzhubu.top/gtidnwmyze.html

[Q79] 字符串拼接
来源：http://hz.hnxiangtu.top/gtskscawot.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.yj20258.top/gtjxxkykql.html

[Q80] 字符串截取
来源：http://hz.guowangkeji.top/gtjpktzujp.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.chenlongwang.top/gtfndtzpmf.html

[Q81] 字符串替换
来源：http://hz.sweek.top/gtognrdjoi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.sxryk.cn/gthvsebsij.html

[Q82] 字符长度与字节长度
来源：http://hz.fengsongda.top/gtmdwwpleb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.fzhhl.top/gtznakzsmz.html

[Q83] 大小写转换
来源：http://hz.jqgfzy.top/gtwswcqdes.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.xylfe.cn/gtnxlcfpmv.html

[Q84] 去除首尾空格
来源：http://hz.gotoacloud.top/gtkpskyspy.html

SELECT TRIM(name) FROM users;
来源：http://hz.xinyue.icu/gtprequxoj.html

[Q85] 数值取整
来源：http://hz.wangshuangyany.cn/gthijgrbpx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.cheryme.top/gtwqykvkth.html

[Q86] 读取 JSON 字段
来源：http://hz.316326.xyz/gtgyaikxhe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.haohaochexian.top/gthykvgvos.html

[Q87] JSON 字段做条件
来源：http://hz.hnqzz.top/gtjtjvhmoh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.guannengcc.top/gtlynqyrbn.html

[Q88] 行转列（条件聚合）
来源：http://hz.tianlin.xyz/gtmsgsjtbs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.tianlin.xyz/gtfssasxee.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.vqdsnc.cn/gtdfcofqjy.html

[Q89] 判断表是否存在
来源：http://hz.yueranfly.top/gtpsdbmyba.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.sweek.top/gtsgrcljtt.html

[Q90] 生成序号列
来源：http://hz.zdqjudy.top/gtqyfqdgif.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.0kj1m.cn/gtcwqaqnxb.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtkrkzltxv.html

R. Bash 专题
来源：http://hz.wangshuangyany.cn/gtnwzcjefw.html

================================================================================
来源：http://hz.nwbrower.top/gttnfrbtiq.html

[R01] shebang 与严格模式
来源：http://hz.jinghuilouyu.cn/gtlvabsajk.html

#!/usr/bin/env bash
来源：http://hz.jinyuanbaomall.cn/gtgumqnues.html

set -euo pipefail
来源：http://hz.daria6918.cn/gtganlgzhm.html

[R02] 变量赋值与使用
来源：http://hz.xylfe.cn/gtrkwwmeqd.html

name="Tom"; echo "$name"
来源：http://hz.tianlin.xyz/gtbwttfwbz.html

[R03] 只读变量
来源：http://hz.daxiang520.top/gtrwoxcvpz.html

readonly PI=3.14
来源：http://hz.chenzaomai.com/gtrzxvaigr.html

[R04] 位置参数
来源：http://hz.ybcxt.top/gtopyapfkw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.mhx1999.top/gtgkttgeon.html

[R05] 参数默认值
来源：http://hz.ehwqpu.com/gtlvwnzmgm.html

name="${1:-default}"
来源：http://hz.pengpengdd.cyou/gtnufqtwra.html

[R06] 判断命令是否存在
来源：http://hz.zhaomingkeji.xyz/gtpcgocdlv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.yangfankeji.com/gtkpmppivu.html

[R07] if 判断文件
来源：http://hz.jqgufenzy.top/gtqauklsdh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydjk.org.cn/gtkcirooem.html

[R08] 数值比较
来源：http://hz.ywan-chungtsiang.top/gtwnhtpjjh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.xuetiantiany.cn/gtlkwfwgmh.html

[R09] 字符串比较
来源：http://hz.ywan-chungtsiang.top/gtxdvclvgp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.hnqzz.top/gtprjgvfsq.html

[R10] 正则匹配
来源：http://hz.jiagoushi.top/gtiucppesv.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.haohaochexian.top/gtzwnbefmc.html

[R11] case 多分支
来源：http://hz.fengsongda.top/gtgndadvfp.html

case "$1" in
来源：http://hz.yanxiufei.cn/gtkbnlcrkg.html

start) echo "启动" ;;
来源：http://hz.hfpthk.cn/gtacqkcmmu.html

stop)  echo "停止" ;;
来源：http://hz.vqdsnc.cn/gttfulqpag.html

*)     echo "未知命令" ;;
来源：http://hz.daxiang520.top/gtjuoefljp.html

esac
来源：http://hz.0kj1m.cn/gtruwlctnq.html

[R12] for 遍历文件
来源：http://hz.zhongyouzk.top/gtxyyixbls.html

for f in *.txt; do echo "$f"; done
来源：http://hz.yangfankeji.com/gtetarfrha.html

[R13] for 计数循环
来源：http://hz.guowangkeji.top/gtulerneed.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.gotoacloud.top/gtianubxln.html

[R14] C 风格 for
来源：http://hz.aizwys.cn/gtqiedgqlh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.haohaochexian.top/gtizbgvxvm.html

[R15] while 逐行读文件
来源：http://hz.bjfxy.top/gtipaozarw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.chenlongwang.top/gtujaibhxo.html

[R16] until 等待条件
来源：http://hz.jinyuanbaomall.cn/gtbmfrebhs.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.nwbrower.top/gtosobyurf.html

[R17] 数组定义与取值
来源：http://hz.yj202588.top/gtnnaolbzq.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.jinqigufen.top/gtdpspqjwe.html

[R18] 遍历数组
来源：http://hz.havefunace.top/gtncflqxxu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.zhengqikj.top/gtyekkdwsf.html

[R19] 数组长度
来源：http://hz.daxiang520.top/gtletajxoz.html

echo "${#arr[@]}"
来源：http://hz.pycfn.com/gtinyovglk.html

[R20] 关联数组（字典）
来源：http://hz.andypj.xyz/gtcmvwhkuk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.jyoumei.cn/gtmftuqeoc.html

[R21] 字符串长度
来源：http://hz.hongshengwenyu.top/gtqywvxudl.html

echo "${#s}"
来源：http://hz.xuetiantiany.cn/gttegvmtse.html

[R22] 截取子串
来源：http://hz.hysaishi.cn/gtkdjjjnro.html

echo "${s:0:5}"
来源：http://hz.gzhubu.top/gtupjltrux.html

[R23] 字符串替换
来源：http://hz.ppjwa.cn/gtevxarveb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.pycfn.com/gtbmshlopj.html

[R24] 大小写转换
来源：http://hz.yueranfly.top/gtpddxzwxn.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.dianchejie.cn/gtyyzjvcug.html

[R25] 去后缀 / 去前缀
来源：http://hz.316326.xyz/gthvemlyxz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.ydzc1.top/gtkxyyykxs.html

[R26] 命令替换
来源：http://hz.yuanzhike.top/gttbaihmvn.html

now=$(date +%F); echo "$now"
来源：http://hz.yueranfly.top/gtdgscycsc.html

[R27] 算术展开
来源：http://hz.fzhhl.top/gtebzkliox.html

echo $((1 + 2 * 3))
来源：http://hz.chenlongwang.top/gtjollaqnw.html

[R28] 浮点运算
来源：http://hz.birdmap.top/gtpblcbada.html

echo "scale=2; 10/3" | bc
来源：http://hz.sysykeji.top/gtsjkrqoom.html

[R29] 定义函数
来源：http://hz.birdmap.top/gtyxbzwdsf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.tanke756.top/gthwduvuzd.html

[R30] 函数返回状态码
来源：http://hz.pycfn.com/gtsuyjiild.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.sufxvd.cn/gtpodhbqnq.html

[R31] 局部变量
来源：http://hz.yuanzhike.top/gtybwckuto.html

f() { local x=1; echo "$x"; }
来源：http://hz.yonumen.top/gtnrmcjevq.html

[R32] 参数个数校验
来源：http://hz.guowangkeji.top/gtvrrejlyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gthbljgnox.html

[R33] 捕获错误并提示行号
来源：http://hz.shanyushiyangkeji.top/gtfxgzwwxx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.yj202588.top/gtkcbhsmvw.html

[R34] 退出时清理
来源：http://hz.0kj1m.cn/gtqcoameqc.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.0kj1m.cn/gtkoqdgxkl.html

[R35] 后台执行并等待
来源：http://hz.mhx1999.top/gtnwcaktoj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.guowangkeji.top/gtjmqnwttg.html

[R36] 并发执行多个任务
来源：http://hz.ydzc1.top/gtlfcduxhr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cucudq.cn/gtxrwrlbjn.html

[R37] 把输出赋给变量
来源：http://hz.tian-w.cn/gtkbhqyioe.html

files=$(ls -1)
来源：http://hz.smart0.xyz/gtmuzsjnib.html

[R38] 管道串联
来源：http://hz.andypj.xyz/gtrtzucuca.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ydjk.org.cn/gtzbuxgatj.html

[R39] 重定向标准输出与错误
来源：http://hz.wangdashe.top/gtiatnufpi.html

cmd > out.log 2>&1
来源：http://hz.smart0.xyz/gtvwrqmojq.html

[R40] 追加写日志
来源：http://hz.yuxming.cn/gtzylvomcq.html

echo "log" >> out.log
来源：http://hz.tian-w.cn/gtdsoquqiu.html

[R41] 丢弃输出
来源：http://hz.birdmap.top/gtdcpxmlky.html

cmd >/dev/null 2>&1
来源：http://hz.nanxinkj.top/gteezwpcsr.html

[R42] 输入重定向
来源：http://hz.cdnleiting.top/gtjtfgcblr.html

wc -l < a.txt
来源：http://hz.yj202588.top/gtyjduvigf.html

[R43] 按名字查找文件
来源：http://hz.smart0.xyz/gthxwkczmx.html

find . -name "*.log" -type f
来源：http://hz.yuxming.cn/gtiywemsvh.html

[R44] 按修改时间查找
来源：http://hz.jyoumei.cn/gtxlypvamz.html

find . -mtime -7 -type f
来源：http://hz.tanke756.top/gtqiuulitf.html

[R45] 批量删除
来源：http://hz.smart0.xyz/gtoofcyyiy.html

find . -name "*.tmp" -delete
来源：http://hz.yj20258888.top/gtreaxcnqk.html

[R46] 递归替换文件内容
来源：http://hz.kuanghao11.cn/gtixtsofeh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.smart0.xyz/gtbrqvohqf.html

[R47] sed 单行替换
来源：http://hz.gaohongyu789.top/gttjcydaqi.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.jinqigfzy.top/gteafirrpd.html

[R48] awk 取指定列
来源：http://hz.daxiang520.top/gtjcxtjmtl.html

awk '{print $1, $3}' a.txt
来源：http://hz.redwolf501.top/gtisgstiwy.html

[R49] awk 带条件
来源：http://hz.hongshengwenyu.top/gtkknxfmqf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.316326.xyz/gtrpebhbau.html

[R50] awk 求和
来源：http://hz.ywan-chungtsiang.top/gtnmybrvco.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.shanyushiyangtech.top/gtqonelgui.html

[R51] 排序去重取前几
来源：http://hz.yj20258888.top/gtjzbxkdud.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hnxiangtu.top/gtdqvyupea.html

[R52] 统计行数
来源：http://hz.cashguo.top/gtqpvyfmte.html

wc -l a.txt
来源：http://hz.ehwqpu.com/gtnehjvyma.html

[R53] 查看文件头与实时尾
来源：http://hz.wangshuangyany.cn/gtrmrtxfoe.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.vqdsnc.cn/gtwbzvuxav.html

[R54] 比较两个文件
来源：http://hz.cqqwz.cn/gtfbwqltqk.html

diff a.txt b.txt
来源：http://hz.haohaochexian.top/gtojqwzhmh.html

[R55] 压缩与解压
来源：http://hz.chenlongwang.top/gtipmsmkvp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.zhixingplan.top/gtaxxuvanv.html

[R56] 远程拷贝
来源：http://hz.dianchejie.cn/gtnfjfxjzm.html

scp file user@host:/path/
来源：http://hz.hywenlv.cn/gtaykonvyf.html

[R57] 远程执行命令
来源：http://hz.xuanzx.com/gthpzqfyym.html

ssh user@host 'uptime'
来源：http://hz.zhijiandao.cn/gtsltwchjv.html

[R58] 下载文件
来源：http://hz.jiagoushi.top/gtjqyknnzc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.yangfankeji.com/gtqypssbwo.html

[R59] 发 POST JSON
来源：http://hz.0kj1m.cn/gtczckxwxp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.yvedp.cn/gtjojxtjyq.html

[R60] 只看 HTTP 状态码
来源：http://hz.yanxiufei.cn/gtdpooiznk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jinghuilouyu.cn/gtzclhttno.html

[R61] 磁盘占用
来源：http://hz.sufxvd.cn/gtfsslxcgi.html

df -h;  du -sh *
来源：http://hz.fengsongda.top/gtigelezgj.html

[R62] 找最占空间的文件
来源：http://hz.snrcjt.cn/gtthkxphql.html

du -ah . | sort -rh | head -10
来源：http://hz.ywan-chungtsiang.top/gtatvktmou.html

[R63] 内存与进程
来源：http://hz.jinyuanbaomall.cn/gtxnjdlbob.html

free -h;  ps aux | grep nginx
来源：http://hz.jinqigfzy.top/gttowtcxmn.html

[R64] 结束进程
来源：http://hz.ivvv.top/gtjrholocc.html

kill -9 $(pgrep -f app.py)
来源：http://hz.yanxiufei.cn/gtoodpgifi.html

[R65] 查看端口占用
来源：http://hz.ivvv.top/gtgjchwmrp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.shzxlz.cn/gtcxubhirx.html

[R66] 定时任务
来源：http://hz.fzhhl.top/gtoizdapwx.html

crontab -e;  crontab -l
来源：http://hz.yuxming.cn/gtodnfebau.html

[R67] 生成随机十六进制串
来源：http://hz.ydjk.org.cn/gthstzgmae.html

openssl rand -hex 16
来源：http://hz.ydjk.org.cn/gtbrwpyfjh.html

[R68] 计算文件校验值
来源：http://hz.shzxlz.cn/gtjbunrqdl.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.wangdashe.top/gtscvgbpca.html

[R69] 生成随机密码
来源：http://hz.cheryme.top/gttzpdlbkb.html

head -c 16 /dev/urandom | base64
来源：http://hz.sxryk.cn/gtpbflxpvk.html

[R70] 时间戳与互转
来源：http://hz.gzhubu.top/gtbtphxjqw.html

date +%s;  date -d @1700000000
来源：http://hz.meibo888.top/gtyicmhsqu.html

[R71] 日期格式化
来源：http://hz.yuanzhike.top/gtfmqncpjl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.snrcjt.cn/gtitzaohpr.html

[R72] 等待端口就绪
来源：http://hz.yuxming.cn/gtvrcahmuj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.meibo888.top/gtuxdilabq.html

[R73] 分割大日志
来源：http://hz.yj20258.top/gtlqzcqniy.html

split -l 1000 big.log part_
来源：http://hz.shangyingyoupin.top/gtumtwmxoj.html

[R74] 批量重命名
来源：http://hz.ppjwa.cn/gtlurqorrw.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.hfpthk.cn/gtwcibccjv.html

[R75] 导出环境变量
来源：http://hz.0kj1m.cn/gthfuochtl.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.hnxiangtu.top/gtfqcilknd.html

[R76] 使用临时文件
来源：http://hz.pycfn.com/gtshznkhwh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.andypj.xyz/gtbkfscmzo.html

[R77] 读取用户输入
来源：http://hz.guowangkeji.top/gtdxknijzc.html

read -rp "请输入: " ans
来源：http://hz.cucudq.cn/gtkamkxxgl.html

[R78] 交互式菜单
来源：http://hz.cqqwz.cn/gtzqvgujck.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.jinqigufen.top/gtrtsbyrrq.html

[R79] 解析命令行选项
来源：http://hz.zhengqikj.top/gtgqogtete.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.yanxiufei.cn/gttvukddcq.html

[R80] 查看脚本执行耗时
来源：http://hz.tanke756.top/gtqmajdquj.html

time ./run.sh
来源：http://hz.xuetiantiany.cn/gtvfsqtvxr.html

================================================================================
来源：http://hz.jlsjyb.cn/gtvjqyipaq.html

S. C / C++ 专题
来源：http://hz.jyoumei.cn/gtfrbrnksc.html

================================================================================
来源：http://hz.xziqi.cn/gtbjlygtxu.html

[S01] C：Hello World
来源：http://hz.jinyuanbaomall.cn/gtrysaogmm.html

#include <stdio.h>
来源：http://hz.c1oappe.top/gtngumwhku.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.gotoacloud.top/gttmgnkqph.html

[S02] C：变量与格式化输出
来源：http://hz.andypj.xyz/gtacbtmele.html

int a = 10; printf("%d\n", a);
来源：http://hz.redwolf501.top/gtwphnodde.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gtbmclbphq.html

int x; scanf("%d", &x);
来源：http://hz.hysaishi.cn/gtzdcchupb.html

[S04] C：字符串复制
来源：http://hz.wangdashe.top/gtjwhzeube.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.xingfuxueyuan.xyz/gtcqrvleep.html

[S05] C：字符串长度
来源：http://hz.sweek.top/gtshoxsiuc.html

strlen(s)
来源：http://hz.mhx1999.top/gttwdsxjor.html

[S06] C：字符串比较
来源：http://hz.chenzaomai.com/gttrvboxvq.html

strcmp(a, b) == 0
来源：http://hz.yj20258.top/gtcfbpncqn.html

[S07] C：数组遍历求和
来源：http://hz.shzxlz.cn/gtbthwlpnw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.gzhubu.top/gthtpaxnec.html

[S08] C：动态内存分配与释放
来源：http://hz.wangdashe.top/gtvoccvacg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.smart0.xyz/gtsuragxsj.html

[S09] C：结构体定义与初始化
来源：http://hz.haohaochexian.top/gtihmgjjdn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.nanxuanxn.top/gtceuztuzu.html

[S10] C：指针与解引用
来源：http://hz.ywan-chungtsiang.top/gtwkqhhcux.html

int *p = &a;  *p = 5;
来源：http://hz.yuxming.cn/gtrbzslifv.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtprchbqql.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.mhx1999.top/gttovdwael.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.smart0.xyz/gtidzivtaf.html

fclose(f);
来源：http://hz.shanyushiyangkeji.top/gtlqllgtuy.html

[S12] C：写文件
来源：http://hz.gzhubu.top/gtajofombt.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.gotoacloud.top/gtnqovhnmp.html

[S13] C：宏定义
来源：http://hz.yj20258888.top/gtjqobslns.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.svipenyu.cn/gtysourjig.html

[S14] C：枚举
来源：http://hz.yueranfly.top/gtceushegn.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.zdqjudy.top/gtbkssujof.html

[S15] C：类型转换
来源：http://hz.hnqzz.top/gtpffiyqtq.html

(double) a / b
来源：http://hz.havefunace.top/gtrqfsttac.html

[S16] C：位操作置位
来源：http://hz.yvedp.cn/gtnktmhdzx.html

x |= (1 << 3);
来源：http://hz.xziqi.cn/gteorepdjh.html

[S17] C：安全拼接字符串
来源：http://hz.gaohongyu789.top/gtldpamrwt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.ivvv.top/gtymwmrisa.html

[S18] C：命令行参数
来源：http://hz.cheryme.top/gtqdvzumie.html

int main(int argc, char **argv)
来源：http://hz.feifeiyinyue.top/gthhrodhsp.html

[S19] C：快速排序
来源：http://hz.zhaomingkeji.xyz/gtukzmzute.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.zdqjudy.top/gtdyvixqpd.html

[S20] C：二分查找
来源：http://hz.52xcode.cn/gtfpbzcjfk.html


<!-- 参考信息 -->