代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.zhijiandao.cn/gtwxslzzxj.html

[Q58] 累计求和
来源：http://hz.havefunace.top/gticwlpyxm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.hammf.cn/gtwwcrcxfi.html

[Q59] 分组内累计
来源：http://hz.hywenlv.cn/gtmjjqgkqp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.tanke756.top/gtemgpjwzh.html

[Q60] 取上一行 / 下一行
来源：http://hz.zhijiandao.cn/gtvnwjzqeb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.redwolf501.top/gtbxwkmfqu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.gogol.net.cn/gtfseflmbx.html

[Q61] 移动平均
来源：http://hz.sweek.top/gtijuyvcjx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.ywan-chungtsiang.top/gtwthtfyle.html

[Q62] 分组占比
来源：http://hz.dashuyun.cn/gtzbtpqjog.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.jyoumei.cn/gtijzqugsa.html

[Q63] 开启事务
来源：http://hz.nwbrower.top/gtigzludzn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.xuetiantiany.cn/gttnlgykef.html

[Q64] 提交事务
来源：http://hz.jlsjyb.cn/gthddcowxa.html

COMMIT;
来源：http://hz.guowangkeji.top/gtrwqetcrq.html

[Q65] 回滚事务
来源：http://hz.ybcxt.top/gtwyvtkowh.html

ROLLBACK;
来源：http://hz.pengpengdd.cyou/gtjwluwihj.html

[Q66] 行锁查询
来源：http://hz.jinghuilouyu.cn/gtmttzlltg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.havefunace.top/gtabjnxbmw.html

[Q67] 设置隔离级别
来源：http://hz.shangyingyoupin.top/gtnwjpvdve.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.yangfankeji.com/gtalvdaqzz.html

[Q68] 保存点
来源：http://hz.hnqzz.top/gtaevgnrtf.html

SAVEPOINT sp1;
来源：http://hz.shangyingyoupin.top/gtjqpeyndm.html

ROLLBACK TO sp1;
来源：http://hz.quarkkingdee.top/gtmmmxwmmp.html

[Q69] 查看执行计划
来源：http://hz.cheryme.top/gtqhycedve.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.aibaodan.cn/gtksosnpca.html

[Q70] 更新统计信息
来源：http://hz.shanyushiyangkeji.top/gtsmcipubp.html

ANALYZE TABLE users;
来源：http://hz.gaohongyu789.top/gtoxlknxyd.html

[Q71] 查看建表语句
来源：http://hz.ywan-chungtsiang.top/gtredderni.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.ydjk.org.cn/gtsxfxfvgx.html

[Q72] 查看索引
来源：http://hz.shuidangran.top/gtiyevcluw.html

SHOW INDEX FROM users;
来源：http://hz.yvedp.cn/gtrjsublfr.html

[Q73] 查看表状态
来源：http://hz.smart0.xyz/gtudsabvqa.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.gaohongyu789.top/gtxbnmazpz.html

[Q74] 强制使用索引
来源：http://hz.yongpay.top/gtfcpdhglw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.feifeiyinyue.top/gtljtbiumi.html

[Q75] 日期格式化
来源：http://hz.nanxinkj.top/gtfbnskwtw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zycfv.cn/gtbyzyamvh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.yuanzhike.top/gtoitdauqs.html

[Q76] 按天统计
来源：http://hz.quarkkingdee.top/gtbjejekvk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.shuidangran.top/gtobgtjafn.html

[Q77] 时间加减
来源：http://hz.sufxvd.cn/gtmprhxfnp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.pengpengdd.cyou/gtkwoxphyp.html

[Q78] 当前时间
来源：http://hz.shuidangran.top/gtnucawszg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.zhoulong.xyz/gtfqrxkncj.html

[Q79] 字符串拼接
来源：http://hz.gzhubu.top/gttaesnjvs.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.dianchejie.cn/gtcciuoprs.html

[Q80] 字符串截取
来源：http://hz.sufxvd.cn/gtnygxedit.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.fzhhl.top/gtnpqolggw.html

[Q81] 字符串替换
来源：http://hz.hysaishi.cn/gtddxtyepu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.vqdsnc.cn/gtierrlwfu.html

[Q82] 字符长度与字节长度
来源：http://hz.jinghuilouyu.cn/gtrlambjhk.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.0kj1m.cn/gtkhplvibo.html

[Q83] 大小写转换
来源：http://hz.dianchejie.cn/gtydpgxgfk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.c1oappe.top/gtmobzxlai.html

[Q84] 去除首尾空格
来源：http://hz.jqgfzy.top/gttkyeplzs.html

SELECT TRIM(name) FROM users;
来源：http://hz.jlsjyb.cn/gtpphhqxtg.html

[Q85] 数值取整
来源：http://hz.ydjk.org.cn/gtrnixxjlj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.svipenyu.cn/gtnlbstcpv.html

[Q86] 读取 JSON 字段
来源：http://hz.xylfe.cn/gtnguxfmcj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.chenlongwang.top/gtrllldtaj.html

[Q87] JSON 字段做条件
来源：http://hz.ydzc1.top/gtzitcttny.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.chenzaomai.com/gtlfktvarv.html

[Q88] 行转列（条件聚合）
来源：http://hz.gogol.net.cn/gtiydqmmlo.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.yvedp.cn/gtxzigatwv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.hnxiangtu.top/gthcbzjgtn.html

[Q89] 判断表是否存在
来源：http://hz.hysaishi.cn/gtghwzebzx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.yonumen.top/gtpbwirsjb.html

[Q90] 生成序号列
来源：http://hz.shanyushiyangkeji.top/gtlbannrmo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.meibo888.top/gtoivcrdkq.html

================================================================================
来源：http://hz.haohaochexian.top/gtawlgvofg.html

R. Bash 专题
来源：http://hz.jqgfzy.top/gtezqsryes.html

================================================================================
来源：http://hz.jqgufenzy.top/gtpoamzcer.html

[R01] shebang 与严格模式
来源：http://hz.zhoulong.xyz/gtadgmxmnl.html

#!/usr/bin/env bash
来源：http://hz.jlsjyb.cn/gtskaprnby.html

set -euo pipefail
来源：http://hz.yuxming.cn/gtacbydhzw.html

[R02] 变量赋值与使用
来源：http://hz.ppjwa.cn/gtawwqlejg.html

name="Tom"; echo "$name"
来源：http://hz.jiagoushi.top/gtdbwkedyf.html

[R03] 只读变量
来源：http://hz.ppjwa.cn/gtjhbxvoqe.html

readonly PI=3.14
来源：http://hz.haohaochexian.top/gtxjcbbdwp.html

[R04] 位置参数
来源：http://hz.kuanghao11.cn/gtjjbsgaxt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.nanxinkj.top/gtzvgfcqfu.html

[R05] 参数默认值
来源：http://hz.52xcode.cn/gtwmmtdlgb.html

name="${1:-default}"
来源：http://hz.tian-w.cn/gtnhfyiyop.html

[R06] 判断命令是否存在
来源：http://hz.smart0.xyz/gtahzttafb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shuidangran.top/gtolwnvkeh.html

[R07] if 判断文件
来源：http://hz.wangdashe.top/gtxgbbqpsu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.ydjk.org.cn/gtphodhdwm.html

[R08] 数值比较
来源：http://hz.sysykeji.top/gtshakvngq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.redwolf501.top/gtkuvjnpba.html

[R09] 字符串比较
来源：http://hz.gzhubu.top/gtucjaiyqw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.andypj.xyz/gtydhhojdy.html

[R10] 正则匹配
来源：http://hz.hywenlv.cn/gtnwzbdnfk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.xinyue.icu/gtnmcbloeg.html

[R11] case 多分支
来源：http://hz.jinghuilouyu.cn/gttkulafln.html

case "$1" in
来源：http://hz.aibaodan.cn/gtmffwvzxf.html

start) echo "启动" ;;
来源：http://hz.ybcxt.top/gtfnlztgvi.html

stop)  echo "停止" ;;
来源：http://hz.yvedp.cn/gtnfcmmjdf.html

*)     echo "未知命令" ;;
来源：http://hz.tanke756.top/gtyokxelmh.html

esac
来源：http://hz.hywenlv.cn/gtqugptwrx.html

[R12] for 遍历文件
来源：http://hz.hfpthk.cn/gtzbeiafdd.html

for f in *.txt; do echo "$f"; done
来源：http://hz.tianlin.xyz/gtmduhzegt.html

[R13] for 计数循环
来源：http://hz.0kj1m.cn/gtfjosbwcv.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.tanke756.top/gtyjebviji.html

[R14] C 风格 for
来源：http://hz.sufxvd.cn/gtvifjgvmb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.shangyingyoupin.top/gtpsutecst.html

[R15] while 逐行读文件
来源：http://hz.ybcxt.top/gtfudlbmsj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.ehwqpu.com/gttnsgjuht.html

[R16] until 等待条件
来源：http://hz.zhoulong.xyz/gtroryxiog.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhoulong.xyz/gthgfjmdjz.html

[R17] 数组定义与取值
来源：http://hz.birdmap.top/gtpyqcikbc.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.yongpay.top/gtpvxalwev.html

[R18] 遍历数组
来源：http://hz.sxryk.cn/gtlwyrgyoj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.chenzaomai.com/gtjiignhwn.html

[R19] 数组长度
来源：http://hz.yuxming.cn/gtgyyxmwbo.html

echo "${#arr[@]}"
来源：http://hz.jinqigufen.top/gtsioipcap.html

[R20] 关联数组（字典）
来源：http://hz.quarkkingdee.top/gtpmvjlamk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.dashuyun.cn/gtfmfrwyxr.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtdwusphjz.html

echo "${#s}"
来源：http://hz.shanyushiyangtech.top/gtrcvofwpk.html

[R22] 截取子串
来源：http://hz.jinqigfzy.top/gtlgknygoy.html

echo "${s:0:5}"
来源：http://hz.zycfv.cn/gtcljbkenq.html

[R23] 字符串替换
来源：http://hz.hnqzz.top/gtakppaveq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.cqqwz.cn/gtpzgijcdz.html

[R24] 大小写转换
来源：http://hz.hongshengwenyu.top/gteyjfnlnw.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.cdnleiting.top/gtrhjlsnth.html

[R25] 去后缀 / 去前缀
来源：http://hz.gotoacloud.top/gtzgiqyqlu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.jqgfzy.top/gtakrilgng.html

[R26] 命令替换
来源：http://hz.pengpengdd.cyou/gtxnlucabl.html

now=$(date +%F); echo "$now"
来源：http://hz.nanxinkj.top/gtjvvuovwd.html

[R27] 算术展开
来源：http://hz.nanxuanxn.top/gtzsbwtbfj.html

echo $((1 + 2 * 3))
来源：http://hz.zhaomingkeji.xyz/gttfxduwcn.html

[R28] 浮点运算
来源：http://hz.xinyue.icu/gtnivpavsq.html

echo "scale=2; 10/3" | bc
来源：http://hz.jinyuanbaomall.cn/gtkzefjmtz.html

[R29] 定义函数
来源：http://hz.cqqwz.cn/gtlmsmhjvo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.sufxvd.cn/gtvinyvhhm.html

[R30] 函数返回状态码
来源：http://hz.gogol.net.cn/gtdnombacd.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.xuanzx.com/gtsbrpgmqi.html

[R31] 局部变量
来源：http://hz.feifeiyinyue.top/gtydklnuhb.html

f() { local x=1; echo "$x"; }
来源：http://hz.yangfankeji.com/gtbnoiqmzd.html

[R32] 参数个数校验
来源：http://hz.cashguo.top/gticiwcqwd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.havefunace.top/gtztxxeubt.html

[R33] 捕获错误并提示行号
来源：http://hz.redwolf501.top/gtihywbzeb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.vqdsnc.cn/gtkebbusdx.html

[R34] 退出时清理
来源：http://hz.wangdashe.top/gthqefwwla.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.pycfn.com/gtchhycsng.html

[R35] 后台执行并等待
来源：http://hz.hysaishi.cn/gtodcoemhe.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.chenzaomai.com/gtsgohxnfx.html

[R36] 并发执行多个任务
来源：http://hz.yueranfly.top/gtushfgrrg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.shuidangran.top/gtfnkjtswi.html

[R37] 把输出赋给变量
来源：http://hz.xinyue.icu/gthrflsizx.html

files=$(ls -1)
来源：http://hz.0kj1m.cn/gtoejpcuqa.html

[R38] 管道串联
来源：http://hz.jinghuilouyu.cn/gtyripblco.html

cat a.txt | grep -i error | wc -l
来源：http://hz.iojbl.cn/gtdhdxaxpt.html

[R39] 重定向标准输出与错误
来源：http://hz.ehwqpu.com/gtdpyqgdge.html

cmd > out.log 2>&1
来源：http://hz.bjfxy.top/gtkzfzfbxz.html

[R40] 追加写日志
来源：http://hz.jianghu66.top/gttrhkmzyo.html

echo "log" >> out.log
来源：http://hz.yj20258.top/gtrsmtvefi.html

[R41] 丢弃输出
来源：http://hz.chenjidiqi.icu/gtjctluwpk.html

cmd >/dev/null 2>&1
来源：http://hz.jlsjyb.cn/gtyflsdexv.html

[R42] 输入重定向
来源：http://hz.xingfuxueyuan.xyz/gtvzknwcxc.html

wc -l < a.txt
来源：http://hz.xinyue.icu/gtcmsifqrg.html

[R43] 按名字查找文件
来源：http://hz.vqdsnc.cn/gtxkabjefq.html

find . -name "*.log" -type f
来源：http://hz.hywenlv.cn/gtaocmddqk.html

[R44] 按修改时间查找
来源：http://hz.sweek.top/gtglkqamtw.html

find . -mtime -7 -type f
来源：http://hz.chenzaomai.com/gtwiozukbu.html

[R45] 批量删除
来源：http://hz.xylfe.cn/gtvxwuieyo.html

find . -name "*.tmp" -delete
来源：http://hz.ydjk.org.cn/gtpudehald.html

[R46] 递归替换文件内容
来源：http://hz.shzxlz.cn/gtqhsmxekv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.0kj1m.cn/gtgsfsidnp.html

[R47] sed 单行替换
来源：http://hz.sxryk.cn/gtgnudwshz.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.yangfankeji.com/gtjjeyysqo.html

[R48] awk 取指定列
来源：http://hz.yj20258888.top/gtbaoiiiyj.html

awk '{print $1, $3}' a.txt
来源：http://hz.cdnleiting.top/gtzlrywack.html

[R49] awk 带条件
来源：http://hz.zhengqikj.top/gthgovtjbq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.zhixingplan.top/gtyuevyvwh.html

[R50] awk 求和
来源：http://hz.jiagoushi.top/gtldxqfhsn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.pycfn.com/gtwhexzlar.html

[R51] 排序去重取前几
来源：http://hz.yongpay.top/gtaszfjnyl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.yuxming.cn/gtgawamdpz.html

[R52] 统计行数
来源：http://hz.hammf.cn/gtfiovkspf.html

wc -l a.txt
来源：http://hz.jinghuilouyu.cn/gtriacczly.html

[R53] 查看文件头与实时尾
来源：http://hz.ivvv.top/gtsdkzavvi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.jqgufenzy.top/gtlzuicamc.html

[R54] 比较两个文件
来源：http://hz.havefunace.top/gtbmlwwufk.html

diff a.txt b.txt
来源：http://hz.zhengqikj.top/gtjuqptehd.html

[R55] 压缩与解压
来源：http://hz.xylfe.cn/gtwhtyirsk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.mhx1999.top/gtpbvzkjdz.html

[R56] 远程拷贝
来源：http://hz.yonumen.top/gtqgretiox.html

scp file user@host:/path/
来源：http://hz.gogol.net.cn/gteifjtjfn.html

[R57] 远程执行命令
来源：http://hz.birdmap.top/gtromerfve.html

ssh user@host 'uptime'
来源：http://hz.mhx1999.top/gtsdbkbwvi.html

[R58] 下载文件
来源：http://hz.jinqigufen.top/gtbrwhyczx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.xinyue.icu/gtoiglowpj.html

[R59] 发 POST JSON
来源：http://hz.c1oappe.top/gtzyuhvdgm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jianghu66.top/gtahmkuwjs.html

[R60] 只看 HTTP 状态码
来源：http://hz.tian-w.cn/gtuhetqzky.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.sxryk.cn/gtxgrfmnto.html

[R61] 磁盘占用
来源：http://hz.xingfuxueyuan.xyz/gtlxivtbis.html

df -h;  du -sh *
来源：http://hz.yvedp.cn/gtxxtrkwsk.html

[R62] 找最占空间的文件
来源：http://hz.gaohongyu789.top/gturhuoree.html

du -ah . | sort -rh | head -10
来源：http://hz.sysykeji.top/gthbqklzco.html

[R63] 内存与进程
来源：http://hz.pengpengdd.cyou/gtmidqctzp.html

free -h;  ps aux | grep nginx
来源：http://hz.yueranfly.top/gtsnskirxb.html

[R64] 结束进程
来源：http://hz.yuxming.cn/gturkpxuan.html

kill -9 $(pgrep -f app.py)
来源：http://hz.shangyingyoupin.top/gtdjkqpzoe.html

[R65] 查看端口占用
来源：http://hz.cucudq.cn/gtajitsslr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.chenjidiqi.icu/gtllfjyigo.html

[R66] 定时任务
来源：http://hz.nanxuanxn.top/gtdiuehztp.html

crontab -e;  crontab -l
来源：http://hz.jqgfzy.top/gtzdlzudye.html

[R67] 生成随机十六进制串
来源：http://hz.ehwqpu.com/gtbeihuraw.html

openssl rand -hex 16
来源：http://hz.zhongyouzk.top/gtvoymdcja.html

[R68] 计算文件校验值
来源：http://hz.ywan-chungtsiang.top/gtcankmfku.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtlqnlwcls.html

[R69] 生成随机密码
来源：http://hz.xinyue.icu/gtvcxskldx.html

head -c 16 /dev/urandom | base64
来源：http://hz.svipenyu.cn/gtfiazbbqg.html

[R70] 时间戳与互转
来源：http://hz.shuidangran.top/gtvnrmhwjk.html

date +%s;  date -d @1700000000
来源：http://hz.kuanghao11.cn/gtrhexugfa.html

[R71] 日期格式化
来源：http://hz.jlsjyb.cn/gtbzmfrcdh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yj202588.top/gtmcweyrdq.html

[R72] 等待端口就绪
来源：http://hz.jqgfzy.top/gtfqtrirgk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.gotoacloud.top/gtwwsqhocm.html

[R73] 分割大日志
来源：http://hz.gotoacloud.top/gtbltibcfk.html

split -l 1000 big.log part_
来源：http://hz.gaohongyu789.top/gtomzsermm.html

[R74] 批量重命名
来源：http://hz.yangfankeji.com/gtksicjvuv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.0kj1m.cn/gtdrtvxrrl.html

[R75] 导出环境变量
来源：http://hz.hongshengwenyu.top/gtshfgyyis.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.pengpengdd.cyou/gttcmybxho.html

[R76] 使用临时文件
来源：http://hz.jinyuanbaomall.cn/gtuuzskfko.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.ppjwa.cn/gtegzyppce.html

[R77] 读取用户输入
来源：http://hz.hammf.cn/gtezgenioa.html

read -rp "请输入: " ans
来源：http://hz.zhongyouzk.top/gtfprxfajq.html

[R78] 交互式菜单
来源：http://hz.jyoumei.cn/gtbvfsxpuu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.chenzaomai.com/gtejyuxzfo.html

[R79] 解析命令行选项
来源：http://hz.smart0.xyz/gtnmpddlds.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jqgufenzy.top/gtgiyenwjr.html

[R80] 查看脚本执行耗时
来源：http://hz.hnxiangtu.top/gtnewynuxv.html

time ./run.sh
来源：http://hz.zhaomingkeji.xyz/gtlobsegxm.html

================================================================================
来源：http://hz.fengsongda.top/gtyxzzxruy.html

S. C / C++ 专题
来源：http://hz.ppjwa.cn/gtiztacquu.html

================================================================================
来源：http://hz.mhx1999.top/gtjakvvlju.html

[S01] C：Hello World
来源：http://hz.vqdsnc.cn/gtagdtpadc.html

#include <stdio.h>
来源：http://hz.feifeiyinyue.top/gtjgajrmrk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.dashuyun.cn/gtmnsqqrjp.html

[S02] C：变量与格式化输出
来源：http://hz.52xcode.cn/gtmmavtopj.html

int a = 10; printf("%d\n", a);
来源：http://hz.jianghu66.top/gtbhqnhclv.html

[S03] C：读入整数
来源：http://hz.zycfv.cn/gtptaehvuz.html

int x; scanf("%d", &x);
来源：http://hz.kuanghao11.cn/gtodurvaif.html

[S04] C：字符串复制
来源：http://hz.yj202588.top/gtpqksgovo.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.hfpthk.cn/gtwmdbjvnp.html

[S05] C：字符串长度
来源：http://hz.xuetiantiany.cn/gtcygmyxyu.html

strlen(s)
来源：http://hz.jinqigufen.top/gtamvztgtr.html

[S06] C：字符串比较
来源：http://hz.zycfv.cn/gtkccxplyo.html

strcmp(a, b) == 0
来源：http://hz.snrcjt.cn/gtlmwigvfe.html

[S07] C：数组遍历求和
来源：http://hz.tanke756.top/gtbgpykuay.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.chenzaomai.com/gtkojvjcdb.html

[S08] C：动态内存分配与释放
来源：http://hz.aibaodan.cn/gthbgovpcn.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.zhaomingkeji.xyz/gtiopeckie.html

[S09] C：结构体定义与初始化
来源：http://hz.gzhubu.top/gtpghiayko.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.xuanzx.com/gttbbtftwb.html

[S10] C：指针与解引用
来源：http://hz.hfpthk.cn/gtamljvdvg.html

int *p = &a;  *p = 5;
来源：http://hz.cashguo.top/gtcpzponlj.html

[S11] C：逐行读文件
来源：http://hz.gogol.net.cn/gtlsaqkwtq.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gtfhfqbval.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.yueranfly.top/gthnpdfmso.html

fclose(f);
来源：http://hz.yvedp.cn/gtyhvnkjma.html

[S12] C：写文件
来源：http://hz.ehwqpu.com/gtpynriujq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yj20258.top/gtgsrimmqd.html

[S13] C：宏定义
来源：http://hz.0kj1m.cn/gtuchjxlli.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.smart0.xyz/gtiunkpaik.html

[S14] C：枚举
来源：http://hz.ydzc1.top/gtjgqledbj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jinqigfzy.top/gthrcsckfq.html

[S15] C：类型转换
来源：http://hz.zycfv.cn/gtinzalyeq.html

(double) a / b
来源：http://hz.guannengcc.top/gthhwswycb.html

[S16] C：位操作置位
来源：http://hz.jianghu66.top/gtrqsselbu.html

x |= (1 << 3);
来源：http://hz.bjfxy.top/gtmevpiinu.html

[S17] C：安全拼接字符串
来源：http://hz.redwolf501.top/gtxqgmdkcn.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.gogol.net.cn/gtzvcqenjy.html

[S18] C：命令行参数
来源：http://hz.yangfankeji.com/gtxvfmlasl.html

int main(int argc, char **argv)
来源：http://hz.andypj.xyz/gtpshpjptb.html

[S19] C：快速排序
来源：http://hz.fengsongda.top/gtlkbzzclw.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.tianlin.xyz/gtlidgxxci.html

[S20] C：二分查找
来源：http://hz.mhx1999.top/gtkbyrydet.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.ppjwa.cn/gtbmuwcwbt.html

[S21] C：字符类别判断
来源：http://hz.fzhhl.top/gtunayjmcd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.yvedp.cn/gtysanlaeo.html

[S22] C：字符串转数字
来源：http://hz.cashguo.top/gtnphzccrm.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.xinyue.icu/gtcftwqztg.html

[S23] C：随机数
来源：http://hz.jinghuilouyu.cn/gtzxdbwhju.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.cqqwz.cn/gtdvdfxgsi.html

[S24] C：获取本地时间
来源：http://hz.zhongyouzk.top/gtoqbeiobr.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.zhoulong.xyz/gtibuflvkn.html

[S25] C：内存拷贝
来源：http://hz.sufxvd.cn/gtyuhqkrhp.html

memcpy(dst, src, n);
来源：http://hz.zhoulong.xyz/gtsrvjjcug.html

[S26] C：内存清零
来源：http://hz.hongshengwenyu.top/gtwxkoyyam.html

memset(a, 0, sizeof a);
来源：http://hz.yuanzhike.top/gtxfwcvtdp.html

[S27] C：定义常量
来源：http://hz.316326.xyz/gtpctvhprk.html

const double PI = 3.14159;
来源：http://hz.gotoacloud.top/gtrhaviehy.html

[S28] C：静态变量
来源：http://hz.cashguo.top/gtllsjthfs.html


<!-- 参考信息 -->