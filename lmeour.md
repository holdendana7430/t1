代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://hz.dashuyun.cn/gtgkuluqje.html

[Q58] 累计求和
来源：http://hz.zhixingplan.top/gtokuugxnj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://hz.xylfe.cn/gtjdslohvb.html

[Q59] 分组内累计
来源：http://hz.c1oappe.top/gtkcpssmzu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://hz.nwbrower.top/gtgbhxajsw.html

[Q60] 取上一行 / 下一行
来源：http://hz.hongshengwenyu.top/gtkxofbcky.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hz.zhoulong.xyz/gtxvqhpebz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://hz.yanxiufei.cn/gtghtrqldq.html

[Q61] 移动平均
来源：http://hz.cdnleiting.top/gtprfmbqqy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://hz.yj20258888.top/gtfldkggbo.html

[Q62] 分组占比
来源：http://hz.jinqigfzy.top/gtctihwian.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://hz.chenlongwang.top/gtkiaoaest.html

[Q63] 开启事务
来源：http://hz.meibo888.top/gtgggjgnjk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.jyoumei.cn/gtmpbomxas.html

[Q64] 提交事务
来源：http://hz.dianchejie.cn/gtisoovfad.html

COMMIT;
来源：http://hz.zycfv.cn/gteuebudtu.html

[Q65] 回滚事务
来源：http://hz.dashuyun.cn/gtunflumen.html

ROLLBACK;
来源：http://hz.cqqwz.cn/gtklnhbdhk.html

[Q66] 行锁查询
来源：http://hz.xylfe.cn/gtdszehvjq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.hywenlv.cn/gtzkzqtbaf.html

[Q67] 设置隔离级别
来源：http://hz.jinqigufen.top/gtxzobxchk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.snrcjt.cn/gtsksdqgwc.html

[Q68] 保存点
来源：http://hz.andypj.xyz/gtibkeozgo.html

SAVEPOINT sp1;
来源：http://hz.havefunace.top/gtbvqynckp.html

ROLLBACK TO sp1;
来源：http://hz.yuanzhike.top/gtywavoymc.html

[Q69] 查看执行计划
来源：http://hz.havefunace.top/gtdofcrrya.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.yongpay.top/gthpezhnub.html

[Q70] 更新统计信息
来源：http://hz.jinyuanbaomall.cn/gttuuyewre.html

ANALYZE TABLE users;
来源：http://hz.zhengqikj.top/gtousnwtkj.html

[Q71] 查看建表语句
来源：http://hz.hnqzz.top/gtzbrjrnll.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.zdqjudy.top/gtucjzdiag.html

[Q72] 查看索引
来源：http://hz.pycfn.com/gtoeyovaqa.html

SHOW INDEX FROM users;
来源：http://hz.cqqwz.cn/gtoxirdlqf.html

[Q73] 查看表状态
来源：http://hz.gaohongyu789.top/gtemvttixu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.feifeiyinyue.top/gthrdrdtpn.html

[Q74] 强制使用索引
来源：http://hz.0kj1m.cn/gtjdwdsmio.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.aibaodan.cn/gtlzwqeecy.html

[Q75] 日期格式化
来源：http://hz.hongshengwenyu.top/gtztaubjbk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.zhongyouzk.top/gthkxmdfrq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.jlsjyb.cn/gtgqbikaht.html

[Q76] 按天统计
来源：http://hz.yvedp.cn/gtjygnvkpz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.jinqigufen.top/gtatdeogmi.html

[Q77] 时间加减
来源：http://hz.guowangkeji.top/gtdyqafqgd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.jyoumei.cn/gtdwpsahhp.html

[Q78] 当前时间
来源：http://hz.ywan-chungtsiang.top/gtvohyaolj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.xziqi.cn/gtscohftze.html

[Q79] 字符串拼接
来源：http://hz.yanxiufei.cn/gtrymapuyi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.cqqwz.cn/gtfyicwuyy.html

[Q80] 字符串截取
来源：http://hz.gaohongyu789.top/gtrkzotsil.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.yangfankeji.com/gtvzhtshve.html

[Q81] 字符串替换
来源：http://hz.mhx1999.top/gtryniadvs.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.hfpthk.cn/gtwiikmzny.html

[Q82] 字符长度与字节长度
来源：http://hz.zhaomingkeji.xyz/gtoopgjxfl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.pengpengdd.cyou/gtakdvytak.html

[Q83] 大小写转换
来源：http://hz.yueranfly.top/gthgujwclg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhiwuduotai.top/gtjygzevab.html

[Q84] 去除首尾空格
来源：http://hz.hnqzz.top/gtewgkfrfr.html

SELECT TRIM(name) FROM users;
来源：http://hz.c1oappe.top/gtdeprdjlm.html

[Q85] 数值取整
来源：http://hz.shuidangran.top/gtdabsyslj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.sweek.top/gtyiofjdgo.html

[Q86] 读取 JSON 字段
来源：http://hz.cqqwz.cn/gtthdaesoc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.fzhhl.top/gtcpotuvqm.html

[Q87] JSON 字段做条件
来源：http://hz.quarkkingdee.top/gteqtwerur.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.jinghuilouyu.cn/gtqpdaluna.html

[Q88] 行转列（条件聚合）
来源：http://hz.cheryme.top/gtcrsmojca.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.sufxvd.cn/gtulmzunjk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.chenlongwang.top/gtoblptyvc.html

[Q89] 判断表是否存在
来源：http://hz.chenjidiqi.icu/gtavkhkvfy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.tian-w.cn/gtwtiajrce.html

[Q90] 生成序号列
来源：http://hz.c1oappe.top/gtilcyhmvo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.tian-w.cn/gtokmggurc.html

================================================================================
来源：http://hz.yuanzhike.top/gttafdekhq.html

R. Bash 专题
来源：http://hz.xingfuxueyuan.xyz/gtymjulgtc.html

================================================================================
来源：http://hz.gzhubu.top/gtqpkvpkpl.html

[R01] shebang 与严格模式
来源：http://hz.nanxinkj.top/gtirczehda.html

#!/usr/bin/env bash
来源：http://hz.hongshengwenyu.top/gtwhclygbj.html

set -euo pipefail
来源：http://hz.zhaomingkeji.xyz/gttrxcokig.html

[R02] 变量赋值与使用
来源：http://hz.xinyue.icu/gtmzombgyn.html

name="Tom"; echo "$name"
来源：http://hz.ivvv.top/gtpzoudycl.html

[R03] 只读变量
来源：http://hz.hnqzz.top/gtxigsnpqi.html

readonly PI=3.14
来源：http://hz.wangshuangyany.cn/gtlabfutcn.html

[R04] 位置参数
来源：http://hz.yueranfly.top/gtsbemsmcx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.jianghu66.top/gtybwitxrj.html

[R05] 参数默认值
来源：http://hz.cqqwz.cn/gtibadmwqr.html

name="${1:-default}"
来源：http://hz.jinyuanbaomall.cn/gtrpojyoyv.html

[R06] 判断命令是否存在
来源：http://hz.kuanghao11.cn/gtbykylkdg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.shanyushiyangtech.top/gtcfbmwbjg.html

[R07] if 判断文件
来源：http://hz.zhixingplan.top/gtmjmwwlry.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.yj202588.top/gtoruzdvys.html

[R08] 数值比较
来源：http://hz.jinqigfzy.top/gtttnnzlsa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.cheryme.top/gtzsnbionw.html

[R09] 字符串比较
来源：http://hz.zdqjudy.top/gtxpxssmic.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.daxiang520.top/gtevidynqz.html

[R10] 正则匹配
来源：http://hz.guannengcc.top/gtmtdrwmjj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.daxiang520.top/gtbpogyilf.html

[R11] case 多分支
来源：http://hz.316326.xyz/gtsefgmror.html

case "$1" in
来源：http://hz.yuxming.cn/gtxmubuoup.html

start) echo "启动" ;;
来源：http://hz.jqgufenzy.top/gtazqlbjfg.html

stop)  echo "停止" ;;
来源：http://hz.yj20258888.top/gtrvuohwun.html

*)     echo "未知命令" ;;
来源：http://hz.zhaomingkeji.xyz/gthdffkxkj.html

esac
来源：http://hz.birdmap.top/gtfnaoncoj.html

[R12] for 遍历文件
来源：http://hz.haohaochexian.top/gthafxyxft.html

for f in *.txt; do echo "$f"; done
来源：http://hz.cheryme.top/gtpzqdgryk.html

[R13] for 计数循环
来源：http://hz.zdqjudy.top/gtbcprwipk.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.fzhhl.top/gtfbzulait.html

[R14] C 风格 for
来源：http://hz.gzhubu.top/gtyufnudpg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.yj202588.top/gtsstyxwhs.html

[R15] while 逐行读文件
来源：http://hz.hnxiangtu.top/gtijhngrek.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.dashuyun.cn/gtjsyuhydb.html

[R16] until 等待条件
来源：http://hz.yangfankeji.com/gtwfvowkff.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.zhongyouzk.top/gtgpwgpruk.html

[R17] 数组定义与取值
来源：http://hz.c1oappe.top/gtmovkjgkb.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.xinyue.icu/gtdnuvwzgi.html

[R18] 遍历数组
来源：http://hz.zhaomingkeji.xyz/gtqufjimgp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.yj202588.top/gtsvimjbql.html

[R19] 数组长度
来源：http://hz.yj20258888.top/gtdrgsxuwa.html

echo "${#arr[@]}"
来源：http://hz.gogol.net.cn/gtqvegglhk.html

[R20] 关联数组（字典）
来源：http://hz.gzhubu.top/gtkrkmeljh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.havefunace.top/gtkfyitmvr.html

[R21] 字符串长度
来源：http://hz.gogol.net.cn/gtttctcrfo.html

echo "${#s}"
来源：http://hz.316326.xyz/gtvprpthmz.html

[R22] 截取子串
来源：http://hz.yonumen.top/gtnvxxrbda.html

echo "${s:0:5}"
来源：http://hz.svipenyu.cn/gtbapcelsv.html

[R23] 字符串替换
来源：http://hz.redwolf501.top/gtbobmkhiw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.jinqigufen.top/gtglsgylzc.html

[R24] 大小写转换
来源：http://hz.kuanghao11.cn/gtktnanhmz.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.gaohongyu789.top/gtueejylyw.html

[R25] 去后缀 / 去前缀
来源：http://hz.cucudq.cn/gtredyajxp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.snrcjt.cn/gtvfqdhwdh.html

[R26] 命令替换
来源：http://hz.tianlin.xyz/gtckkittsm.html

now=$(date +%F); echo "$now"
来源：http://hz.feifeiyinyue.top/gtggqsbzlm.html

[R27] 算术展开
来源：http://hz.jinqigfzy.top/gtagasjalv.html

echo $((1 + 2 * 3))
来源：http://hz.mhx1999.top/gtozbatuie.html

[R28] 浮点运算
来源：http://hz.nwbrower.top/gtxpfypuyc.html

echo "scale=2; 10/3" | bc
来源：http://hz.hongshengwenyu.top/gtkcjlpeaz.html

[R29] 定义函数
来源：http://hz.xuetiantiany.cn/gtsljvsnnx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.kuanghao11.cn/gtsrsvcipa.html

[R30] 函数返回状态码
来源：http://hz.jinqigufen.top/gtbhctyqfs.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.jianghu66.top/gtpnupkqan.html

[R31] 局部变量
来源：http://hz.jinqigfzy.top/gtwdlcwmue.html

f() { local x=1; echo "$x"; }
来源：http://hz.chenlongwang.top/gtuolkruen.html

[R32] 参数个数校验
来源：http://hz.ppjwa.cn/gtghbmvfks.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.jqgufenzy.top/gtzsvcfoba.html

[R33] 捕获错误并提示行号
来源：http://hz.andypj.xyz/gtbqachqtw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.ydjk.org.cn/gtaskgfopr.html

[R34] 退出时清理
来源：http://hz.ivvv.top/gtdrdxudig.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.52xcode.cn/gtolgfpoal.html

[R35] 后台执行并等待
来源：http://hz.quarkkingdee.top/gtkjxnmnmy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.tanke756.top/gtojavqtyv.html

[R36] 并发执行多个任务
来源：http://hz.zhengqikj.top/gtrchauxju.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.cashguo.top/gtqsweybxg.html

[R37] 把输出赋给变量
来源：http://hz.yvedp.cn/gtaqpetjfe.html

files=$(ls -1)
来源：http://hz.sxryk.cn/gtzdfdregn.html

[R38] 管道串联
来源：http://hz.9152youxi.cn/gttlxrtoxd.html

cat a.txt | grep -i error | wc -l
来源：http://hz.daxiang520.top/gtgozjjxpo.html

[R39] 重定向标准输出与错误
来源：http://hz.hnxiangtu.top/gtfzibjrtt.html

cmd > out.log 2>&1
来源：http://hz.ywan-chungtsiang.top/gtmtyyxwpy.html

[R40] 追加写日志
来源：http://hz.hysaishi.cn/gtywruhpos.html

echo "log" >> out.log
来源：http://hz.gogol.net.cn/gtpbjpvtrb.html

[R41] 丢弃输出
来源：http://hz.xziqi.cn/gtadzxckfb.html

cmd >/dev/null 2>&1
来源：http://hz.yueranfly.top/gthxuuvvsx.html

[R42] 输入重定向
来源：http://hz.yongpay.top/gtkujmslcy.html

wc -l < a.txt
来源：http://hz.cdnleiting.top/gtnekajpew.html

[R43] 按名字查找文件
来源：http://hz.yuanzhike.top/gtzxgmncqc.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtlncuface.html

[R44] 按修改时间查找
来源：http://hz.meibo888.top/gtxbtqhfxg.html

find . -mtime -7 -type f
来源：http://hz.gogol.net.cn/gtdhymjssm.html

[R45] 批量删除
来源：http://hz.tianlin.xyz/gtibjblzhj.html

find . -name "*.tmp" -delete
来源：http://hz.birdmap.top/gtotufgclq.html

[R46] 递归替换文件内容
来源：http://hz.quarkkingdee.top/gtrdfrvpfd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.gzhubu.top/gteoeittzn.html

[R47] sed 单行替换
来源：http://hz.xingfuxueyuan.xyz/gtnpjnxwqg.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.bjfxy.top/gtpnuzzowj.html

[R48] awk 取指定列
来源：http://hz.hysaishi.cn/gtsjuotftv.html

awk '{print $1, $3}' a.txt
来源：http://hz.jyoumei.cn/gtnevjqwsj.html

[R49] awk 带条件
来源：http://hz.ydzc1.top/gtzrorpkjk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.shzxlz.cn/gtxwyvayxm.html

[R50] awk 求和
来源：http://hz.snrcjt.cn/gtviyezfqn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yj20258888.top/gtotsyaghm.html

[R51] 排序去重取前几
来源：http://hz.jlsjyb.cn/gtxczyhujr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.wangdashe.top/gtdtogpyje.html

[R52] 统计行数
来源：http://hz.sxryk.cn/gtliloizev.html

wc -l a.txt
来源：http://hz.iojbl.cn/gtgkbotwpn.html

[R53] 查看文件头与实时尾
来源：http://hz.yj20258.top/gtpgaafrvy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.sxryk.cn/gtkcdpoktj.html

[R54] 比较两个文件
来源：http://hz.sweek.top/gtuzuecwfy.html

diff a.txt b.txt
来源：http://hz.sufxvd.cn/gtckqddyxc.html

[R55] 压缩与解压
来源：http://hz.jqgufenzy.top/gtcjmubguc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.xuetiantiany.cn/gtogfkmnwj.html

[R56] 远程拷贝
来源：http://hz.pycfn.com/gtnjahfkxy.html

scp file user@host:/path/
来源：http://hz.sysykeji.top/gtaflinxpz.html

[R57] 远程执行命令
来源：http://hz.jqgfzy.top/gtmudwxtjj.html

ssh user@host 'uptime'
来源：http://hz.tianlin.xyz/gtyyssaxcm.html

[R58] 下载文件
来源：http://hz.ydjk.org.cn/gtggztmgwe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.nwbrower.top/gtxskzdeva.html

[R59] 发 POST JSON
来源：http://hz.zhaomingkeji.xyz/gtloewpyox.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.pycfn.com/gtnzevbuwg.html

[R60] 只看 HTTP 状态码
来源：http://hz.xingfuxueyuan.xyz/gtkyuccvru.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jianghu66.top/gtpjqzznqv.html

[R61] 磁盘占用
来源：http://hz.redwolf501.top/gtplauxcor.html

df -h;  du -sh *
来源：http://hz.316326.xyz/gtftszhjfs.html

[R62] 找最占空间的文件
来源：http://hz.aibaodan.cn/gtynnyjieb.html

du -ah . | sort -rh | head -10
来源：http://hz.0kj1m.cn/gtfrwpjexh.html

[R63] 内存与进程
来源：http://hz.nwbrower.top/gteelpgzpj.html

free -h;  ps aux | grep nginx
来源：http://hz.jlsjyb.cn/gtrhugkejc.html

[R64] 结束进程
来源：http://hz.pengpengdd.cyou/gtisiefhjm.html

kill -9 $(pgrep -f app.py)
来源：http://hz.52xcode.cn/gtxdwvausv.html

[R65] 查看端口占用
来源：http://hz.cashguo.top/gtdisxthmj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.yj20258.top/gtpeodjhff.html

[R66] 定时任务
来源：http://hz.vqdsnc.cn/gtcyzmitrp.html

crontab -e;  crontab -l
来源：http://hz.feifeiyinyue.top/gtlnjzbfbl.html

[R67] 生成随机十六进制串
来源：http://hz.sysykeji.top/gtlnbsngtn.html

openssl rand -hex 16
来源：http://hz.cqqwz.cn/gtgzlfrsek.html

[R68] 计算文件校验值
来源：http://hz.kuanghao11.cn/gtweqazepz.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.cdnleiting.top/gtchipfvnx.html

[R69] 生成随机密码
来源：http://hz.tanke756.top/gtrydlzqmo.html

head -c 16 /dev/urandom | base64
来源：http://hz.shuidangran.top/gtzxwtkzyf.html

[R70] 时间戳与互转
来源：http://hz.cucudq.cn/gtoppfqvaq.html

date +%s;  date -d @1700000000
来源：http://hz.yonumen.top/gtnpfgxqcn.html

[R71] 日期格式化
来源：http://hz.ybcxt.top/gtsegmocmy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.yongpay.top/gtemdyjxyk.html

[R72] 等待端口就绪
来源：http://hz.daria6918.cn/gtyirkwpka.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.kuanghao11.cn/gtuapgyawq.html

[R73] 分割大日志
来源：http://hz.snrcjt.cn/gtlcdgcbgr.html

split -l 1000 big.log part_
来源：http://hz.andypj.xyz/gtsescukli.html

[R74] 批量重命名
来源：http://hz.shanyushiyangtech.top/gtdwbgiowh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.zdqjudy.top/gtgiplqtcl.html

[R75] 导出环境变量
来源：http://hz.316326.xyz/gtpycklxdt.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.wangdashe.top/gtezvhpeab.html

[R76] 使用临时文件
来源：http://hz.tian-w.cn/gtscjryvxa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.xziqi.cn/gtcyrvsvio.html

[R77] 读取用户输入
来源：http://hz.cucudq.cn/gtjsllbgqt.html

read -rp "请输入: " ans
来源：http://hz.tian-w.cn/gtsounupdg.html

[R78] 交互式菜单
来源：http://hz.nanxuanxn.top/gtwsoppenw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.xziqi.cn/gtdunicyxn.html

[R79] 解析命令行选项
来源：http://hz.quarkkingdee.top/gtewmrwert.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.jiagoushi.top/gtolvzyeut.html

[R80] 查看脚本执行耗时
来源：http://hz.andypj.xyz/gtekrrvwya.html

time ./run.sh
来源：http://hz.chenlongwang.top/gtfyinlksq.html

================================================================================
来源：http://hz.kuanghao11.cn/gtxndnqvwp.html

S. C / C++ 专题
来源：http://hz.fzhhl.top/gtmmxkefjx.html

================================================================================
来源：http://hz.haohaochexian.top/gtorlmauuo.html

[S01] C：Hello World
来源：http://hz.sweek.top/gtvlpdukxn.html

#include <stdio.h>
来源：http://hz.9152youxi.cn/gtedsskbzr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.tian-w.cn/gtilfmvvzm.html

[S02] C：变量与格式化输出
来源：http://hz.yanxiufei.cn/gtcrhzimdi.html

int a = 10; printf("%d\n", a);
来源：http://hz.ydzc1.top/gtwapdkbtu.html

[S03] C：读入整数
来源：http://hz.316326.xyz/gtfyecvsrp.html

int x; scanf("%d", &x);
来源：http://hz.nwbrower.top/gthyvuqmfg.html

[S04] C：字符串复制
来源：http://hz.wangshuangyany.cn/gtkxqmxfvv.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.zhiwuduotai.top/gtdvxmmgue.html

[S05] C：字符串长度
来源：http://hz.yongpay.top/gtoakqnqpw.html

strlen(s)
来源：http://hz.jianghu66.top/gtzjutouog.html

[S06] C：字符串比较
来源：http://hz.guowangkeji.top/gtashsbrhe.html

strcmp(a, b) == 0
来源：http://hz.xylfe.cn/gtdlbvjuot.html

[S07] C：数组遍历求和
来源：http://hz.wangshuangyany.cn/gthdubydgt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.xinyue.icu/gtuywmdvpa.html

[S08] C：动态内存分配与释放
来源：http://hz.zhiwuduotai.top/gtgegzglea.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.jinqigfzy.top/gtwylfkgkv.html

[S09] C：结构体定义与初始化
来源：http://hz.aibaodan.cn/gtewjiasin.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.feifeiyinyue.top/gtttwxjfqa.html

[S10] C：指针与解引用
来源：http://hz.jinghuilouyu.cn/gtoekyqzop.html

int *p = &a;  *p = 5;
来源：http://hz.fengsongda.top/gtnzylnpwg.html

[S11] C：逐行读文件
来源：http://hz.dashuyun.cn/gtzxrktaea.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.cqqwz.cn/gthidfnovq.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.dashuyun.cn/gtocqctxpu.html

fclose(f);
来源：http://hz.hywenlv.cn/gtuiskzunr.html

[S12] C：写文件
来源：http://hz.andypj.xyz/gtoikukdeu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.jinyuanbaomall.cn/gtnrxrsjlb.html

[S13] C：宏定义
来源：http://hz.yvedp.cn/gtkxndponl.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.cqqwz.cn/gtgrfrrljy.html

[S14] C：枚举
来源：http://hz.zhijiandao.cn/gtmlxlnwdy.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.jqgfzy.top/gtcktnhkxo.html

[S15] C：类型转换
来源：http://hz.havefunace.top/gtlspxgfid.html

(double) a / b
来源：http://hz.jqgfzy.top/gtugzhwjfz.html

[S16] C：位操作置位
来源：http://hz.wangshuangyany.cn/gthfslvpsp.html

x |= (1 << 3);
来源：http://hz.andypj.xyz/gtyycmzcfk.html

[S17] C：安全拼接字符串
来源：http://hz.cdnleiting.top/gtikxyligq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.hfpthk.cn/gtlcycfjtc.html

[S18] C：命令行参数
来源：http://hz.ywan-chungtsiang.top/gtgpawpqgx.html

int main(int argc, char **argv)
来源：http://hz.tian-w.cn/gtmuwnloiy.html

[S19] C：快速排序
来源：http://hz.aizwys.cn/gtrcqpxnkm.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.nanxuanxn.top/gttipeoopt.html

[S20] C：二分查找
来源：http://hz.sxryk.cn/gtgtwfmejs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.fzhhl.top/gtvzliuagn.html

[S21] C：字符类别判断
来源：http://hz.jinghuilouyu.cn/gtqhaptrqb.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.nanxuanxn.top/gthgifjfzc.html

[S22] C：字符串转数字
来源：http://hz.wangdashe.top/gtyumfweik.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.dianchejie.cn/gtttsmdgew.html

[S23] C：随机数
来源：http://hz.jyoumei.cn/gtopabbflc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.hnxiangtu.top/gtgzowhwek.html

[S24] C：获取本地时间
来源：http://hz.zhixingplan.top/gtaataigzz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.cashguo.top/gtsvbzichr.html

[S25] C：内存拷贝
来源：http://hz.guowangkeji.top/gtnwxmlrus.html

memcpy(dst, src, n);
来源：http://hz.52xcode.cn/gttzgllhvo.html

[S26] C：内存清零
来源：http://hz.sufxvd.cn/gtlrwxbywq.html

memset(a, 0, sizeof a);
来源：http://hz.zhiwuduotai.top/gtrnrhpppj.html

[S27] C：定义常量
来源：http://hz.fzhhl.top/gtxamidrwc.html

const double PI = 3.14159;
来源：http://hz.zhongyouzk.top/gtmwwttcik.html

[S28] C：静态变量
来源：http://hz.gogol.net.cn/gthhfyendj.html


<!-- 参考信息 -->