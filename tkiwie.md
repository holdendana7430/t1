代发 wailian999

[Q63] 开启事务
来源：http://hz.yongpay.top/gtomfmxigk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://hz.yongpay.top/gtgsvowdjy.html

[Q64] 提交事务
来源：http://hz.zhiwuduotai.top/gtbdbbmuew.html

COMMIT;
来源：http://hz.yvedp.cn/gtdmrhjfox.html

[Q65] 回滚事务
来源：http://hz.zhijiandao.cn/gtknguzpgp.html

ROLLBACK;
来源：http://hz.andypj.xyz/gtsizrmpfj.html

[Q66] 行锁查询
来源：http://hz.hywenlv.cn/gtmqwcggdh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://hz.vqdsnc.cn/gtrlkduspf.html

[Q67] 设置隔离级别
来源：http://hz.chenjidiqi.icu/gtoahujpuc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hz.havefunace.top/gtrdjtkgjo.html

[Q68] 保存点
来源：http://hz.xuanzx.com/gtjxoidvaa.html

SAVEPOINT sp1;
来源：http://hz.jinqigufen.top/gtqpkjodxi.html

ROLLBACK TO sp1;
来源：http://hz.shanyushiyangtech.top/gteqdzajyk.html

[Q69] 查看执行计划
来源：http://hz.chenlongwang.top/gtlzbiucgk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://hz.zhengqikj.top/gtevahkrla.html

[Q70] 更新统计信息
来源：http://hz.ydzc1.top/gtatdsxmme.html

ANALYZE TABLE users;
来源：http://hz.ivvv.top/gtzjhusugj.html

[Q71] 查看建表语句
来源：http://hz.yanxiufei.cn/gttuilpojj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hz.nanxinkj.top/gtegzpvyog.html

[Q72] 查看索引
来源：http://hz.ydjk.org.cn/gtjcmdxikv.html

SHOW INDEX FROM users;
来源：http://hz.hfpthk.cn/gtmvigctld.html

[Q73] 查看表状态
来源：http://hz.jinqigfzy.top/gtcvmaulxj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://hz.cashguo.top/gtxovobpqs.html

[Q74] 强制使用索引
来源：http://hz.shanyushiyangtech.top/gtvlynsfna.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://hz.gotoacloud.top/gtyjlrlibt.html

[Q75] 日期格式化
来源：http://hz.cqqwz.cn/gtnyjltyfj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://hz.0kj1m.cn/gtvdikxeic.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://hz.sxryk.cn/gtkyexjwkk.html

[Q76] 按天统计
来源：http://hz.yj20258.top/gtohaqpexe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://hz.andypj.xyz/gtrcgymlez.html

[Q77] 时间加减
来源：http://hz.shangyingyoupin.top/gtmsfpbwom.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://hz.sufxvd.cn/gtqzppmfup.html

[Q78] 当前时间
来源：http://hz.ehwqpu.com/gtvyaqzzvz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hz.jqgufenzy.top/gthxlkkqfr.html

[Q79] 字符串拼接
来源：http://hz.zhengqikj.top/gtvlpesamr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://hz.jqgfzy.top/gtdxbrnjrb.html

[Q80] 字符串截取
来源：http://hz.jiagoushi.top/gtxazooaei.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://hz.shzxlz.cn/gtqsywawki.html

[Q81] 字符串替换
来源：http://hz.meibo888.top/gtimvmhhhy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://hz.nwbrower.top/gthiezecoz.html

[Q82] 字符长度与字节长度
来源：http://hz.hysaishi.cn/gtuvfajvux.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtqheolufs.html

[Q83] 大小写转换
来源：http://hz.pengpengdd.cyou/gtpxgzumxm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://hz.zhixingplan.top/gtozlkvvtb.html

[Q84] 去除首尾空格
来源：http://hz.shanyushiyangtech.top/gthyczzkdr.html

SELECT TRIM(name) FROM users;
来源：http://hz.xingfuxueyuan.xyz/gtglzmdqqx.html

[Q85] 数值取整
来源：http://hz.jyoumei.cn/gtejoujofo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://hz.tanke756.top/gtgfaibevb.html

[Q86] 读取 JSON 字段
来源：http://hz.dianchejie.cn/gtlygqhwno.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://hz.cdnleiting.top/gtpiwgjyef.html

[Q87] JSON 字段做条件
来源：http://hz.andypj.xyz/gtmxpootoq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://hz.svipenyu.cn/gtobbogvky.html

[Q88] 行转列（条件聚合）
来源：http://hz.ydjk.org.cn/gttbbdjvlh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://hz.chenlongwang.top/gtdeafexir.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hz.ywan-chungtsiang.top/gtzwlmlhuy.html

[Q89] 判断表是否存在
来源：http://hz.yanxiufei.cn/gtpichzyrz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://hz.vqdsnc.cn/gtdvywapsc.html

[Q90] 生成序号列
来源：http://hz.yuxming.cn/gtqyczkplj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://hz.yueranfly.top/gtioehndzx.html

================================================================================
来源：http://hz.9152youxi.cn/gtbvtzrzaw.html

R. Bash 专题
来源：http://hz.ywan-chungtsiang.top/gtznolybif.html

================================================================================
来源：http://hz.cucudq.cn/gtlgbyqmmv.html

[R01] shebang 与严格模式
来源：http://hz.pycfn.com/gtnhmfcczk.html

#!/usr/bin/env bash
来源：http://hz.redwolf501.top/gtplkazjpv.html

set -euo pipefail
来源：http://hz.xinyue.icu/gtipknprpk.html

[R02] 变量赋值与使用
来源：http://hz.daxiang520.top/gtgyzzhenb.html

name="Tom"; echo "$name"
来源：http://hz.hammf.cn/gtxvxmnras.html

[R03] 只读变量
来源：http://hz.quarkkingdee.top/gtfwijputz.html

readonly PI=3.14
来源：http://hz.snrcjt.cn/gtqaqvfxjz.html

[R04] 位置参数
来源：http://hz.sweek.top/gtotwisrnz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://hz.xylfe.cn/gtubaiisph.html

[R05] 参数默认值
来源：http://hz.sufxvd.cn/gtjufynonn.html

name="${1:-default}"
来源：http://hz.yueranfly.top/gtvsccjfbm.html

[R06] 判断命令是否存在
来源：http://hz.hnxiangtu.top/gtbwejwjcm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://hz.chenzaomai.com/gtuzyxsgye.html

[R07] if 判断文件
来源：http://hz.haohaochexian.top/gtnufqsnkb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hz.zhoulong.xyz/gtgpxrlnvq.html

[R08] 数值比较
来源：http://hz.snrcjt.cn/gtrevioogn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://hz.sweek.top/gtkonqrhmw.html

[R09] 字符串比较
来源：http://hz.sysykeji.top/gtujdcddju.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://hz.iojbl.cn/gtnzcpebfl.html

[R10] 正则匹配
来源：http://hz.jqgfzy.top/gtavuttixo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://hz.yj202588.top/gtpptezuzi.html

[R11] case 多分支
来源：http://hz.zhoulong.xyz/gtnrtkcvmd.html

case "$1" in
来源：http://hz.zhixingplan.top/gtffuvhqld.html

start) echo "启动" ;;
来源：http://hz.dashuyun.cn/gttjjunyji.html

stop)  echo "停止" ;;
来源：http://hz.cdnleiting.top/gtnyqnktif.html

*)     echo "未知命令" ;;
来源：http://hz.ivvv.top/gtnehcqzmm.html

esac
来源：http://hz.pengpengdd.cyou/gtdkygectq.html

[R12] for 遍历文件
来源：http://hz.cqqwz.cn/gtnwhkzxkr.html

for f in *.txt; do echo "$f"; done
来源：http://hz.shanyushiyangkeji.top/gtohhcngot.html

[R13] for 计数循环
来源：http://hz.52xcode.cn/gtzvttwjnc.html

for i in {1..10}; do echo "$i"; done
来源：http://hz.jinqigufen.top/gtzoauckpr.html

[R14] C 风格 for
来源：http://hz.cucudq.cn/gteeqrucfq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://hz.xinyue.icu/gtsichzvgf.html

[R15] while 逐行读文件
来源：http://hz.shanyushiyangtech.top/gtchkhdprh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hz.xingfuxueyuan.xyz/gtbtulcqkr.html

[R16] until 等待条件
来源：http://hz.dianchejie.cn/gtchfzibhd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://hz.ppjwa.cn/gttcuyxrqf.html

[R17] 数组定义与取值
来源：http://hz.nwbrower.top/gtxgyaqdex.html

arr=(a b c); echo "${arr[0]}"
来源：http://hz.haohaochexian.top/gtlshzmzyg.html

[R18] 遍历数组
来源：http://hz.ybcxt.top/gtdicachqr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://hz.ybcxt.top/gtumwgzqze.html

[R19] 数组长度
来源：http://hz.snrcjt.cn/gtmqykqopa.html

echo "${#arr[@]}"
来源：http://hz.snrcjt.cn/gttgfacehx.html

[R20] 关联数组（字典）
来源：http://hz.jqgfzy.top/gtfsornpqg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://hz.ywan-chungtsiang.top/gtarmxzcwm.html

[R21] 字符串长度
来源：http://hz.snrcjt.cn/gtvshlukgr.html

echo "${#s}"
来源：http://hz.nanxinkj.top/gtiqguecho.html

[R22] 截取子串
来源：http://hz.svipenyu.cn/gtvsrjrmun.html

echo "${s:0:5}"
来源：http://hz.birdmap.top/gtdlnwoyat.html

[R23] 字符串替换
来源：http://hz.shanyushiyangkeji.top/gtnzxiikoq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://hz.ybcxt.top/gtyqsnhuvf.html

[R24] 大小写转换
来源：http://hz.nanxuanxn.top/gtzinbgumg.html

echo "${s^^}"; echo "${s,,}"
来源：http://hz.xuetiantiany.cn/gtfhochpce.html

[R25] 去后缀 / 去前缀
来源：http://hz.yonumen.top/gtmzxgsmwv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://hz.dashuyun.cn/gtqqlrpxih.html

[R26] 命令替换
来源：http://hz.fzhhl.top/gthfkgvjcl.html

now=$(date +%F); echo "$now"
来源：http://hz.jqgfzy.top/gtwrpqautc.html

[R27] 算术展开
来源：http://hz.cqqwz.cn/gtrytbkfal.html

echo $((1 + 2 * 3))
来源：http://hz.guowangkeji.top/gtodwpcraf.html

[R28] 浮点运算
来源：http://hz.zdqjudy.top/gtzjiorvgs.html

echo "scale=2; 10/3" | bc
来源：http://hz.xuetiantiany.cn/gtsxeymwwy.html

[R29] 定义函数
来源：http://hz.cashguo.top/gtxigqscgs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://hz.iojbl.cn/gttcabavwb.html

[R30] 函数返回状态码
来源：http://hz.9152youxi.cn/gtwvvbygjp.html

f() { return 0; }; f || echo "失败了"
来源：http://hz.tian-w.cn/gtekdzryvq.html

[R31] 局部变量
来源：http://hz.andypj.xyz/gtohemimjt.html

f() { local x=1; echo "$x"; }
来源：http://hz.xinyue.icu/gtizrefgif.html

[R32] 参数个数校验
来源：http://hz.smart0.xyz/gttzgjdzwq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://hz.52xcode.cn/gtmmfmqfyy.html

[R33] 捕获错误并提示行号
来源：http://hz.snrcjt.cn/gtzwmgiise.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://hz.shuidangran.top/gtqblvdgia.html

[R34] 退出时清理
来源：http://hz.ydjk.org.cn/gtwtutsupd.html

trap 'rm -f "$tmp"' EXIT
来源：http://hz.wangshuangyany.cn/gtfszcnzww.html

[R35] 后台执行并等待
来源：http://hz.daria6918.cn/gtwvlhklgw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://hz.hongshengwenyu.top/gtvifnlrtf.html

[R36] 并发执行多个任务
来源：http://hz.jyoumei.cn/gtohbyyior.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://hz.ivvv.top/gtvtpvdima.html

[R37] 把输出赋给变量
来源：http://hz.ehwqpu.com/gtpgmjznrn.html

files=$(ls -1)
来源：http://hz.xuetiantiany.cn/gtsgahmukx.html

[R38] 管道串联
来源：http://hz.sweek.top/gtwpvlpokv.html

cat a.txt | grep -i error | wc -l
来源：http://hz.ybcxt.top/gtsmyqcdmq.html

[R39] 重定向标准输出与错误
来源：http://hz.yj20258.top/gtarpvlryz.html

cmd > out.log 2>&1
来源：http://hz.havefunace.top/gtfcnbisrp.html

[R40] 追加写日志
来源：http://hz.zhixingplan.top/gtocpgibri.html

echo "log" >> out.log
来源：http://hz.yangfankeji.com/gtqwahgdcm.html

[R41] 丢弃输出
来源：http://hz.hnqzz.top/gtcasfxqaw.html

cmd >/dev/null 2>&1
来源：http://hz.dianchejie.cn/gtfqmzlobl.html

[R42] 输入重定向
来源：http://hz.tanke756.top/gtfupmokho.html

wc -l < a.txt
来源：http://hz.xylfe.cn/gtipetsfna.html

[R43] 按名字查找文件
来源：http://hz.ywan-chungtsiang.top/gtieekzlgv.html

find . -name "*.log" -type f
来源：http://hz.zhoulong.xyz/gtbukdavxj.html

[R44] 按修改时间查找
来源：http://hz.yj202588.top/gtzmxiyovn.html

find . -mtime -7 -type f
来源：http://hz.hysaishi.cn/gtjabysbga.html

[R45] 批量删除
来源：http://hz.wangshuangyany.cn/gtthieofuv.html

find . -name "*.tmp" -delete
来源：http://hz.havefunace.top/gtchdozqhp.html

[R46] 递归替换文件内容
来源：http://hz.ppjwa.cn/gtmcfxkcpz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://hz.ivvv.top/gtbgznytjs.html

[R47] sed 单行替换
来源：http://hz.9152youxi.cn/gtmnwqctie.html

sed -i 's/foo/bar/g' a.txt
来源：http://hz.zycfv.cn/gtddzbrrvr.html

[R48] awk 取指定列
来源：http://hz.wangshuangyany.cn/gtmxupppjx.html

awk '{print $1, $3}' a.txt
来源：http://hz.sufxvd.cn/gtujevrbbi.html

[R49] awk 带条件
来源：http://hz.hywenlv.cn/gtjindcwnl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://hz.mhx1999.top/gtxpcldxhb.html

[R50] awk 求和
来源：http://hz.sysykeji.top/gtrwevpazn.html

awk '{s += $2} END {print s}' a.txt
来源：http://hz.yonumen.top/gtezvtpzca.html

[R51] 排序去重取前几
来源：http://hz.tanke756.top/gtcttbqzch.html

sort a.txt | uniq -c | sort -rn | head
来源：http://hz.hfpthk.cn/gtdpgtbadk.html

[R52] 统计行数
来源：http://hz.chenjidiqi.icu/gtnthgadla.html

wc -l a.txt
来源：http://hz.nanxinkj.top/gtxngsllnd.html

[R53] 查看文件头与实时尾
来源：http://hz.jiagoushi.top/gtxzaorhhm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hz.hfpthk.cn/gtikqskkeq.html

[R54] 比较两个文件
来源：http://hz.xuanzx.com/gttsigcxxy.html

diff a.txt b.txt
来源：http://hz.daria6918.cn/gtssdarzfq.html

[R55] 压缩与解压
来源：http://hz.jqgfzy.top/gtphidoens.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hz.dianchejie.cn/gtuqytkfbx.html

[R56] 远程拷贝
来源：http://hz.iojbl.cn/gtsumrhovb.html

scp file user@host:/path/
来源：http://hz.xinyue.icu/gtrvluujfo.html

[R57] 远程执行命令
来源：http://hz.fzhhl.top/gtiwgrudjc.html

ssh user@host 'uptime'
来源：http://hz.9152youxi.cn/gttzqfvxly.html

[R58] 下载文件
来源：http://hz.yuanzhike.top/gtneqzclfd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hz.vqdsnc.cn/gtbyatvcjk.html

[R59] 发 POST JSON
来源：http://hz.pycfn.com/gtzsdgccpb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hz.jinyuanbaomall.cn/gtaupvplcq.html

[R60] 只看 HTTP 状态码
来源：http://hz.shuidangran.top/gtctxtocjm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://hz.jqgufenzy.top/gtwsefufid.html

[R61] 磁盘占用
来源：http://hz.c1oappe.top/gtuhwuzdyu.html

df -h;  du -sh *
来源：http://hz.gzhubu.top/gtfqyxrmhs.html

[R62] 找最占空间的文件
来源：http://hz.zhoulong.xyz/gtijaiaqlt.html

du -ah . | sort -rh | head -10
来源：http://hz.birdmap.top/gtpvdfgmwv.html

[R63] 内存与进程
来源：http://hz.52xcode.cn/gtufitjsox.html

free -h;  ps aux | grep nginx
来源：http://hz.ivvv.top/gtecimglqa.html

[R64] 结束进程
来源：http://hz.jinghuilouyu.cn/gtvrrbdfxi.html

kill -9 $(pgrep -f app.py)
来源：http://hz.jinyuanbaomall.cn/gtocsyxhof.html

[R65] 查看端口占用
来源：http://hz.tianlin.xyz/gtqyyfmfqv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hz.daxiang520.top/gtuyrhrcwh.html

[R66] 定时任务
来源：http://hz.zhaomingkeji.xyz/gttyctvtpo.html

crontab -e;  crontab -l
来源：http://hz.zhijiandao.cn/gternmtwty.html

[R67] 生成随机十六进制串
来源：http://hz.chenzaomai.com/gtcvolqoll.html

openssl rand -hex 16
来源：http://hz.tian-w.cn/gthxvlmjqq.html

[R68] 计算文件校验值
来源：http://hz.zhaomingkeji.xyz/gtaxgqqbxd.html

sha256sum a.txt;  md5sum a.txt
来源：http://hz.0kj1m.cn/gtafbelahw.html

[R69] 生成随机密码
来源：http://hz.jqgfzy.top/gtopavowih.html

head -c 16 /dev/urandom | base64
来源：http://hz.fzhhl.top/gtggjlriln.html

[R70] 时间戳与互转
来源：http://hz.andypj.xyz/gtjhgvngjg.html

date +%s;  date -d @1700000000
来源：http://hz.xylfe.cn/gtzdovqnpt.html

[R71] 日期格式化
来源：http://hz.jinqigufen.top/gtutluedcy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://hz.jiagoushi.top/gtdoqvhvul.html

[R72] 等待端口就绪
来源：http://hz.yvedp.cn/gtjzdcmtjg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://hz.sysykeji.top/gtsyceeavo.html

[R73] 分割大日志
来源：http://hz.jianghu66.top/gtxcilhchv.html

split -l 1000 big.log part_
来源：http://hz.yangfankeji.com/gtallizhyr.html

[R74] 批量重命名
来源：http://hz.jqgufenzy.top/gtsolmdkfb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hz.meibo888.top/gtxazrwadc.html

[R75] 导出环境变量
来源：http://hz.fzhhl.top/gtblxbqkxf.html

export PATH="$HOME/bin:$PATH"
来源：http://hz.yj20258.top/gtudynumsv.html

[R76] 使用临时文件
来源：http://hz.jianghu66.top/gtbmptzwxj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hz.cucudq.cn/gtdelzzozg.html

[R77] 读取用户输入
来源：http://hz.yueranfly.top/gthinhjaqv.html

read -rp "请输入: " ans
来源：http://hz.shangyingyoupin.top/gthcmtbthu.html

[R78] 交互式菜单
来源：http://hz.shanyushiyangtech.top/gtchuptacv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://hz.hnqzz.top/gtdglwkhvv.html

[R79] 解析命令行选项
来源：http://hz.hnxiangtu.top/gttphcrnoa.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hz.fzhhl.top/gtoxgjynyl.html

[R80] 查看脚本执行耗时
来源：http://hz.zhengqikj.top/gtccagrech.html

time ./run.sh
来源：http://hz.fengsongda.top/gtchelwkdu.html

================================================================================
来源：http://hz.iojbl.cn/gttkcxglcw.html

S. C / C++ 专题
来源：http://hz.tianlin.xyz/gtijykbnkl.html

================================================================================
来源：http://hz.yj20258.top/gtqrojbqzb.html

[S01] C：Hello World
来源：http://hz.xinyue.icu/gtzvclhrek.html

#include <stdio.h>
来源：http://hz.cashguo.top/gttgmboogt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://hz.fzhhl.top/gttjgljfyt.html

[S02] C：变量与格式化输出
来源：http://hz.wangdashe.top/gtuuzdegfa.html

int a = 10; printf("%d\n", a);
来源：http://hz.shzxlz.cn/gthgtixdil.html

[S03] C：读入整数
来源：http://hz.andypj.xyz/gtgtbjiqbt.html

int x; scanf("%d", &x);
来源：http://hz.yueranfly.top/gtatmnxjdz.html

[S04] C：字符串复制
来源：http://hz.shanyushiyangkeji.top/gtcutlmbzg.html

char dst[32]; strcpy(dst, "hi");
来源：http://hz.vqdsnc.cn/gtcnuwulro.html

[S05] C：字符串长度
来源：http://hz.ybcxt.top/gtybzjwcds.html

strlen(s)
来源：http://hz.jinqigufen.top/gtjcawtedr.html

[S06] C：字符串比较
来源：http://hz.xinyue.icu/gtgjxrmfsp.html

strcmp(a, b) == 0
来源：http://hz.yueranfly.top/gtrojyunwq.html

[S07] C：数组遍历求和
来源：http://hz.jyoumei.cn/gtbnwvvxmy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hz.yanxiufei.cn/gtbfddumjt.html

[S08] C：动态内存分配与释放
来源：http://hz.ydzc1.top/gtazhfjqsp.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hz.yj202588.top/gtdcyzzknv.html

[S09] C：结构体定义与初始化
来源：http://hz.hnqzz.top/gtajhxhxtw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hz.ehwqpu.com/gtbsjuwxfg.html

[S10] C：指针与解引用
来源：http://hz.yuanzhike.top/gtirkeawmn.html

int *p = &a;  *p = 5;
来源：http://hz.jinyuanbaomall.cn/gtbijcjtlc.html

[S11] C：逐行读文件
来源：http://hz.havefunace.top/gtklpeqerz.html

FILE *f = fopen("a.txt", "r");
来源：http://hz.pengpengdd.cyou/gtfqupqscj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://hz.9152youxi.cn/gtnxaglipz.html

fclose(f);
来源：http://hz.yanxiufei.cn/gtafgnclzk.html

[S12] C：写文件
来源：http://hz.jinqigfzy.top/gtqiuwcyuh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hz.yvedp.cn/gtwptbohir.html

[S13] C：宏定义
来源：http://hz.jyoumei.cn/gteqjvjkby.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hz.tanke756.top/gtivktfggl.html

[S14] C：枚举
来源：http://hz.xuanzx.com/gtduwlbfzj.html

enum Color { RED, GREEN, BLUE };
来源：http://hz.nwbrower.top/gthacybouu.html

[S15] C：类型转换
来源：http://hz.jinghuilouyu.cn/gtfdberoua.html

(double) a / b
来源：http://hz.kuanghao11.cn/gttgjpetny.html

[S16] C：位操作置位
来源：http://hz.aizwys.cn/gtcsakfjck.html

x |= (1 << 3);
来源：http://hz.sufxvd.cn/gtvvpffcsm.html

[S17] C：安全拼接字符串
来源：http://hz.ppjwa.cn/gtkauniwmg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hz.52xcode.cn/gtjhjilubz.html

[S18] C：命令行参数
来源：http://hz.c1oappe.top/gtmzqihhzx.html

int main(int argc, char **argv)
来源：http://hz.mhx1999.top/gthflsxorx.html

[S19] C：快速排序
来源：http://hz.ppjwa.cn/gtcbuwpqsr.html

qsort(a, n, sizeof(int), cmp);
来源：http://hz.52xcode.cn/gtckdnkeyl.html

[S20] C：二分查找
来源：http://hz.xuanzx.com/gtsnyqfhet.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hz.zhongyouzk.top/gtyhkjrmtw.html

[S21] C：字符类别判断
来源：http://hz.c1oappe.top/gtupwgkdry.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hz.shangyingyoupin.top/gtrvizeada.html

[S22] C：字符串转数字
来源：http://hz.fengsongda.top/gtzwlghoaa.html

atoi("42");  strtod("3.14", NULL);
来源：http://hz.hysaishi.cn/gtiawfampy.html

[S23] C：随机数
来源：http://hz.jianghu66.top/gtvcirscex.html

srand(time(NULL));  int r = rand() % 100;
来源：http://hz.pycfn.com/gtxjkesuaj.html

[S24] C：获取本地时间
来源：http://hz.gzhubu.top/gtxfnzspbn.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hz.kuanghao11.cn/gtssheyjgp.html

[S25] C：内存拷贝
来源：http://hz.zhoulong.xyz/gttbezmypc.html

memcpy(dst, src, n);
来源：http://hz.zhiwuduotai.top/gtnwpnoxrw.html

[S26] C：内存清零
来源：http://hz.9152youxi.cn/gtohpxnibw.html

memset(a, 0, sizeof a);
来源：http://hz.guowangkeji.top/gtffxpaswr.html

[S27] C：定义常量
来源：http://hz.zhijiandao.cn/gttmwoygxm.html

const double PI = 3.14159;
来源：http://hz.zdqjudy.top/gtofgjsjyn.html

[S28] C：静态变量
来源：http://hz.hfpthk.cn/gtjcrktyne.html

static int counter = 0;
来源：http://hz.cheryme.top/gtxnivskqq.html

[S29] C：变参函数
来源：http://hz.tian-w.cn/gtqrmfhxmt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hz.nanxinkj.top/gtvlgtvqui.html

[S30] C：头文件保护
来源：http://hz.xuetiantiany.cn/gtzceojqsr.html

#ifndef X_H
来源：http://hz.yuxming.cn/gtwymhqrvr.html

#define X_H
来源：http://hz.svipenyu.cn/gtjnzktvxf.html

#endif
来源：http://hz.hfpthk.cn/gtkfrygzam.html

[S31] C++：Hello World
来源：http://hz.fengsongda.top/gthynmtrry.html

#include <iostream>
来源：http://hz.yanxiufei.cn/gtpvxcyutp.html

int main() { std::cout << "Hello\n"; }
来源：http://hz.daria6918.cn/gtdbpfwkfi.html

[S32] C++：字符串
来源：http://hz.zdqjudy.top/gtdtztqngu.html

std::string s = "hi";  s += "!";
来源：http://hz.yongpay.top/gtfobznkta.html


<!-- 参考信息 -->