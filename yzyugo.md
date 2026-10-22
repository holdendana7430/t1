代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mafsuvxx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fgwqkcng.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2vlovzpki.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrijjuwz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xersrjaz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lpeixtpa.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2adpxquuf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2uomepnto.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zpbxxazx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2qrzemgjm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2piodlowi.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2hgkdqjce.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2vkvzzolf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2alfgmnfp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vkymlrjw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2eujaaozw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2kdcvhtvn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vevhxuvk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2gxepscdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ikcnihou.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2umyljchc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qcdzqadq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2zdiuzdqi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jfvosvdj.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2dxqxdexd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2paznwruj.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2aqjsdphl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ftoztndt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2scqpshmo.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ikgchvsb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2cndjdnpg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2sdserjke.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2bnzmgiqn.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jlnyaluf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lqpsojrw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2vwrtpeso.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ojhifouz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ieikfzsr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jilzqbld.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dxbygmnu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ngrskdbe.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vnitkzid.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yjbyxkcb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mlztlzcl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rdgrzlsl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nnmoqraz.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2liuwefha.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dylsikqc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2qhtwibmm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2ivrhqorg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2azmnebrn.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xyebvuag.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2byssojsv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2duvnauqk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rzyxtlns.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hwaglopg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ziarfsot.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2fiblatza.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rcxmucix.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rtrqpkoa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nmhcpomm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2pgcmreto.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfueauxz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fnhumecu.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ibirzajm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wmrlvimt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hzlxeqjd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2hxydfrwo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2uemosngb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ropgktjg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2jowywrrd.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tndktcoa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qidqmuuc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vkyvibxe.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uowqnjkc.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wynoidho.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ylbxugqc.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2ejjpkzjo.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2rdpnrdqc.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ugwqhgzo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ncrbwzqm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2meaxkiwv.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2wmxrklao.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2muaemcrz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ocpmrwsq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yoaagubo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2gzkpxozb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2ikcfdrfn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kuwwyyqz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2dzpxxssv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pxcpzvpg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2ixrzljbf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rethgbay.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ikenljtv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yprcnkji.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zvgkdrpc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lqepaygy.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fszxdfrt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2azotcxab.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hqjjvghm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2tywboaaa.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qapbcuur.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2tuttrcym.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rjrikkwc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2skojppok.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2tscpvysp.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ljffywur.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gmfcdcdh.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nektfnoj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qbtknuax.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vymjdvlt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2dkfkcjqm.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yzraodto.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2owkhmxfk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kqpjjjxh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2mqzthbck.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kovbiodo.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2lthlphns.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2uxbcrzgs.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2xxactuyd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smajtovo.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ejbwnoum.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jtbjwmps.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2puafnknd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2geknmxii.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2eluptgvq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ookuglmq.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rqspslrc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hkrrwudh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ilahqkhr.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2afdnranl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2hatkoker.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2pkidssdy.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vdjmoizf.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zmzfmtid.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2lduuurhl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2tkotbvwc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lugwcxyp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pwadoolz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2pxinzjiy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hrmskwxm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2euwfkqyj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2kvzmrfgx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hbgkwyej.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qjlwphxb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2iorkaxai.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gxifdrwy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ezbsevlo.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gdyfvfdz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2eicxezwl.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2aouzzmnd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dyhttcbu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2pvmraluv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xmbdtgid.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kmhwhlhq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2pzaxhvoo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ojbvtvqv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2njhddxvd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lykihjtm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pxlrrptd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wxjqcjwb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2vcgsluln.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fduhylxn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2cxyrajdu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2kjlvrslc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vfendjlr.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2alhzqzwp.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2gwmspduo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cajiqcnp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2wjsocivn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ovjoyprr.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ltyvjqfz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2htlrhqwh.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2papmzrmv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ncynaues.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hnrmiksx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2ydomjzqe.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2zlwamjem.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2saoiiuxq.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mjygmbbh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2hgbmkxwp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wyypepig.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jquhvnep.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2quzkuzrp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2xutnhvsv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2tecnytku.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zqzisqqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tpgshtuq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2mywvdjfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uksradlo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqidil.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2fjugcjol.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2msfxcgpq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2kkxzugah.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2lloyvkjm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xcaqaulf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2hndokdgq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2fbmcbvto.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tcphhebp.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xnanuzyj.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2mkotvdav.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2dtwdpgce.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2xenvbjtt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gjduwrcl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2iaycyfow.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ixsqgmkd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2doilzxfw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hghyyfyb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2sciayivl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2foyrxtwu.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ypymenrx.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wxmxstpt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fgdocyvd.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ympteulj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jxsixlyt.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2grpkwopu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2xroxmvsg.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vwwwzfxn.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2drqprwrj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2pcclnvza.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dygxsxll.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2zuxqjzlb.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ymrrzacc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2cmfmzvww.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2yqtikzyy.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2niedlejk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hdbtmwce.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2gvzikjia.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2namwduvx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2vxlecesi.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2opyxjupt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rtwfjidv.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2folcygek.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2xkjxyrzp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kyhvylxr.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ngyclurk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2spcpjkbl.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2eqbdiosp.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2oovaoduj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zaixyfla.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ncqjqhfp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2jcdstgwk.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2outssrsf.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2momvitwd.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2xajtxdjr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2bgdivjqm.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gxmempzo.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2chwqjcik.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2phibzolu.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2retzmxsf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2zatswwoi.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ggsyuszd.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ipnnttwf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2bqvgyenz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ufrriqmt.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2afmguiuq.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2cqboprbn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2evizjojq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2crrwvlpi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ucxoakmh.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2waevolrf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2woxvgsei.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2afcyngku.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmfkqhsq.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2mxywsjkm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cmrhdjtp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2zqcrncnx.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fjamvzid.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2grcojsjf.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hpccsccb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2lrnipuoa.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gwywpsvy.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2sjjtncnf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2vvykypcs.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2mtkeejwg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2mijmdxfj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zikmuoow.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2uxmyfwxe.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2itoodgpw.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qiywupiw.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2cbejybdm.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fwuhjfuy.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2xcroyojs.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2vaisghey.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2fjzagkcm.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ylrrqgpw.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2lorxqxzf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ccrombyr.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2thzpoqva.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2urlccngt.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xuvrxptf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rkpciebz.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2fxqklvnh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rrudssod.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2noaeucfi.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2tokyfmqy.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2fbtptuuu.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2clrzferm.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jqvcftqd.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2oxjieknp.html


<!-- 参考信息 -->